Breast Cancer Diagnosis using SVM

This project uses Support Vector Machine (SVM) to classify breast cancer tumors as Malignant or Benign.

Dataset

- File: data.csv
- Target column: diagnosis
- M → 1 (Malignant)
- B → 0 (Benign)
- Dropped columns: id, Unnamed: 32

Libraries Used

- pandas
- numpy
- matplotlib
- scikit-learn
- joblib

Workflow

- Load and preprocess data
- Encode target labels
- Split data into training and testing sets
- Standardize features
- Train SVM with linear and RBF kernels
- Tune hyperparameters using GridSearchCV
- Evaluate model using accuracy, confusion matrix, classification report
- Plot ROC curve and calculate AUC score
- Save trained model as a pipeline

Installation
pip install pandas numpy matplotlib scikit-learn joblib

Run
python svm_model.py

Output

- Model accuracy
- Best hyperparameters
- Classification report
- Confusion matrix
- ROC curve and AUC score
- Saved model file
  Saved Model
  svm_breast_cancer_model.pkl

Load Model
import joblib  
model = joblib.load("svm_breast_cancer_model.pkl")
