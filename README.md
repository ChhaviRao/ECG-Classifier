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

## Model Performance

The selected model is a voting ensemble combining SVM, XGBoost, and AdaBoost.

| Metric | Result |
|---|---:|
| Test Accuracy | 86.32% |
| Balanced Accuracy | 56.87% |
| Macro F1-Score | 51.61% |

## Limitations

The dataset has an imbalanced class distribution, which affects performance across heartbeat categories. This project is an educational machine learning prototype and is **not intended for clinical diagnosis**.

## Future Improvements

- Improve minority-class detection.
- Add explainable AI (XAI) using SHAP.
- Develop an interactive web interface for predictions.
- Evaluate the model with additional validation techniques.
## Future Improvements

- Improve recognition of minority heartbeat classes.
- Add explainability using SHAP or other XAI techniques.
- Develop a user-friendly prediction interface.
- Evaluate generalization on additional independent datasets.
