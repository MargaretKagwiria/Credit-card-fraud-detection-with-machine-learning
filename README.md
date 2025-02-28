# Credit Card Fraud Detection using Machine Learning

## Overview
This project applies machine learning techniques to detect fraudulent credit card transactions. The dataset used is the **Credit Card Fraud Detection dataset** from Kaggle, which contains anonymized transaction data.

## Dataset
- The dataset consists of numerical features obtained using **Principal Component Analysis (PCA)**.
- The `Time` column is removed as it does not provide meaningful insights.
- The `Amount` column is standardized to improve model performance.
- The target variable (`Class`) has two values:
  - `0`: Legitimate transactions
  - `1`: Fraudulent transactions
- The dataset is highly imbalanced, requiring special handling techniques.

## Technologies Used
- **Python**
- **Pandas, NumPy** (Data manipulation)
- **Scikit-learn** (Machine learning models and evaluation)
- **imbalanced-learn (SMOTE)** (Handling class imbalance)
- **XGBoost** (Boosting classifier)
- **Matplotlib, Seaborn** (Data visualization)

## Steps in the Project
1. **Exploratory Data Analysis (EDA)**: Understanding dataset structure, class distribution, and statistics.
2. **Data Preprocessing**: Removing unnecessary features, standardizing numerical columns.
3. **Handling Class Imbalance**: Applying **Synthetic Minority Over-sampling Technique (SMOTE)**.
4. **Splitting Data**: Separating dataset into training and testing sets.
5. **Model Training**:
   - Logistic Regression
   - Random Forest Classifier
   - XGBoost Classifier
6. **Model Evaluation**:
   - **Classification Report** (Precision, Recall, F1-Score)
   - **AUC-ROC Score**
   - **Confusion Matrix**
7. **Comparison of Models**

## Results
| Model  | Precision | Recall | F1-Score | AUC-ROC |
|--------|----------|--------|----------|---------|
| Logistic Regression | 92% | 67% | 77% | 0.90 |
| Random Forest | 96% | 85% | 90% | 0.97 |
| XGBoost | 98% | 88% | 93% | 0.98 |

- **XGBoost performed the best**, achieving high recall and F1-score.
- **SMOTE significantly improved model performance** by balancing the dataset.
- **Random Forest and XGBoost outperformed Logistic Regression** in detecting fraudulent transactions.

## Installation & Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/MargaretKagwiria/credit-card-fraud-detection.git
   cd credit-card-fraud-detection

