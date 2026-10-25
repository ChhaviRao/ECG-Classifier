# ECG Classifier — ECG Lens

## Project Overview

ECG Lens is a machine learning project that classifies electrocardiogram (ECG) heartbeats into four categories using the MIT-BIH Arrhythmia Database.

The project explores how traditional machine learning algorithms and ensemble learning can help classify ECG heartbeat patterns.

## Classes

- **N:** Normal and related beats
- **S:** Supraventricular ectopic beats
- **V:** Ventricular ectopic beats
- **F:** Fusion beats

## Machine Learning Models

The selected model is a voting ensemble combining:

- Support Vector Machine (SVM)
- XGBoost
- AdaBoost

The pipeline uses 226 engineered features derived from ECG waveforms and heartbeat timing information.

## Project Files

- `ECG_Classifier_Training.ipynb` — model training and evaluation
- `ECG_Classifier_Prediction.ipynb` — prediction workflow
- `ecg_lens_model_bundle.joblib` — saved model bundle
- `ECG_Classifier_Project_Guide.docx` — experiment and viva guide

## Dataset

The project uses the MIT-BIH Arrhythmia Database. Please follow the dataset provider's access conditions and citation requirements.

## Evaluation

The original experiment reported:

- Test accuracy: **86.32%**
- Test balanced accuracy: **56.87%**
- Test macro-F1 score: **0.5161**

Accuracy alone does not reflect performance equally across all classes, particularly because the dataset is imbalanced.

## Technologies

Python, NumPy, Pandas, SciPy, scikit-learn, XGBoost, WFDB, and Jupyter Notebook.

## Limitations

This project is an educational and research prototype. It is not a clinically validated system and must not be used to diagnose heart conditions or make medical decisions.

## Future Improvements

- Improve recognition of minority heartbeat classes.
- Add explainability using SHAP or other XAI techniques.
- Develop a user-friendly prediction interface.
- Evaluate generalization on additional independent datasets.
