# Breast Cancer Classification using Machine Learning

## Project Overview
This project applies data analytics and machine learning techniques on the Breast Cancer Wisconsin dataset to classify tumors as **Benign (B)** or **Malignant (M)**.  
The workflow includes data preprocessing, exploratory data analysis (EDA), feature engineering, and supervised learning model training.

---

## Objectives
- **Perform data analysis and feature engineering** to understand important predictors in breast cancer diagnosis.  
- **Build and evaluate machine learning models** (Logistic Regression, Random Forest, SVM) to classify breast cancer with high accuracy.

---

## Dataset
- Source: Breast Cancer Wisconsin (Diagnostic) Dataset (available via `sklearn.datasets` or Kaggle).  
- Features: 30 numeric attributes (radius, perimeter, concavity, etc.).  
- Target: `diagnosis` → Benign (B) or Malignant (M).  

---

## Methods
1. **Data Cleaning**  
   - Removed duplicate/unnecessary columns (like `Unnamed: 32`).  
   - Checked for missing values.  

2. **Exploratory Data Analysis (EDA)**  
   - Box plots, histograms, skewness, and correlation analysis.  
   - Identified most important features (e.g., `area_worst`, `radius_mean`).  

3. **Feature Engineering**  
   - Encoded target labels (`B=0`, `M=1`).  
   - Standardized features using `StandardScaler`.  

4. **Model Training & Evaluation**  
   - Logistic Regression  
   - Random Forest  
   - Support Vector Machine (SVM)  

---

## Results
| Model                | Accuracy | Benign Recall | Malignant Recall |
|----------------------|----------|---------------|------------------|
| Logistic Regression  | 0.9649   | 0.99          | 0.93             |
| Random Forest        | 0.9737   | 1.00          | 0.93             |
| SVM (RBF kernel)     | 0.9737   | 1.00          | 0.93             |

- Random Forest and SVM gave the best performance.  
- Important features included **area_worst, concave points_worst, radius_worst, perimeter_mean**.  

---

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/breast-cancer-ml-project.git
   cd breast-cancer-ml-project
