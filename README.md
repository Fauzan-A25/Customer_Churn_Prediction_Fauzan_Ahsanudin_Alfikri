# 📉 Customer Churn Prediction Challenge

## 🧑‍💼 Overview

This project aims to predict customer churn using a machine learning model trained on structured customer data. It was developed as part of the **Customer Churn Prediction Challenge** organized by GDGOC Telkom University. Early churn detection enables businesses to take proactive measures to retain at-risk customers and improve long-term profitability.

## 👤 Author

- **Name**: Fauzan Ahsanudin Alfikri  
- **NIM**: 103052300003

## 📂 Dataset

The dataset is split into:
- `train.csv`: Contains historical customer data along with the target label `churn`.
- `test.csv`: Contains new customer records without churn labels, used for model inference.

Key features in the dataset include:
- Categorical: `gender`, `region`, `membership_category`, etc.
- Numerical: `joining_date`, `last_visit_time`, `past_3_years_bike_related_purchases`, etc.

## 🔧 Preprocessing

The following steps were performed:
- **Missing Value Handling**: Used `KNNImputer` to handle missing numerical data.
- **Label Encoding**: Applied to categorical columns for compatibility with scikit-learn models.
- **Feature-Target Split**: Data was split into `X` and `y` for model training.

## 🧠 Model

- **Algorithm Used**: Random Forest Classifier (`sklearn.ensemble.RandomForestClassifier`)
- **Evaluation Metrics**:
  - **F1-Score**
  - **Classification Report**
  - **Confusion Matrix**

The model was trained using an 80-20 train-test split and evaluated using the F1-score, which balances precision and recall—particularly important for imbalanced classes like churn prediction.

## 📈 Results

The model demonstrated strong performance on the training dataset. Detailed metrics from the evaluation:
- Precision, Recall, and F1-Score for both churned and non-churned classes.
- Confusion matrix to visualize classification performance.

## 📌 Features of the Solution

- Robust missing value imputation using **KNNImputer**.
- **LabelEncoder** to transform categorical values efficiently.
- Evaluation through detailed metrics to identify potential overfitting or underfitting.
- Exported final predictions to CSV for submission or further analysis.

## 🚀 How to Run

1. Clone this repository.
2. Ensure you have the required libraries:
   ```bash
   pip install pandas scikit-learn
Run the notebook: Customer_Churn_Prediction_Challenge_Fauzan_Ahsanudin_Alfikri.ipynb in Jupyter Notebook or Google Colab.

Replace the file paths to point to your local or cloud storage if needed.

## 📌 Future Improvements
Hyperparameter tuning using GridSearchCV or RandomizedSearchCV.

Experiment with ensemble models like XGBoost or LightGBM.

Feature engineering to improve model robustness and interpretability.

Incorporate SHAP or LIME for explainability.

## 📚 Acknowledgments
Special thanks to Google Developer Student Clubs Telkom University for organizing the challenge and providing a platform to apply practical machine learning skills.
