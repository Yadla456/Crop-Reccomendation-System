# Crop-Reccomendation-System

## Overview
The Crop Recommendation System is designed to assist farmers and agricultural professionals in identifying the most suitable crop to cultivate based on environmental factors. Using machine learning algorithms, the system provides highly accurate crop recommendations by analyzing various features such as soil characteristics, temperature, and humidity.

---

## Features
- Preprocessing of data using outlier removal techniques (IQR and clipping).
- Multi-algorithm model training:
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM)
  - Random Forest
- Finalized the Random Forest model with **99.73% accuracy**.
- Detailed evaluation metrics including accuracy, precision, recall, F1-score, and confusion matrix.

---

## Dataset
The dataset contains crop-specific data such as:
- **Numerical Features**: Soil characteristics, temperature, humidity, etc.
- **Labels**: Crop types (e.g., banana, maize, rice, etc.).

Preprocessing steps:
1. Outlier removal using mean ± 3*std.
2. Encoding categorical crop labels using `LabelEncoder`.



## Code Description
### Preprocessing
- **Outlier Removal**: Clipping data outside mean ± 3*std to handle anomalies.
- **Label Encoding**: Converts crop names into numerical labels for model compatibility.

### Model Training
- **Logistic Regression**: Baseline model for linear classification.
- **KNN**: Distance-based algorithm for non-linear data.
- **SVM**: Kernel-based approach for complex decision boundaries.
- **Random Forest**: Final model selected for its robustness and high accuracy.

### Evaluation Metrics
- **Classification Report**: Precision, recall, and F1-score for each crop class.
- **Confusion Matrix**: Visual representation of model predictions vs. actual values.


## Requirements
### Programming Language
- Python 3.7+

### Libraries
- `pandas` for data handling.
- `numpy` for numerical computations.
- `scikit-learn` for machine learning models and evaluation.
- `matplotlib` and `seaborn` for visualization.

Install required libraries:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```


## Results
- Final model: **Random Forest**
- **Accuracy**: 99.73%
- **Classification Report**: Shows high precision, recall, and F1-scores for all crop types.

---

## Limitations
- Dataset size may limit the generalizability of the model.
- SVM and KNN are computationally expensive for larger datasets.

---

## Future Enhancements
- Incorporate crop rotation and sustainability factors into the recommendation system.
- Extend the dataset with more diverse geographical and climatic data.

