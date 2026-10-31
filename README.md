# Credit-Scoring-System

# Credit Scoring System

An end-to-end Machine Learning application that predicts loan default risk based on applicant and loan information. This project covers data preprocessing, exploratory data analysis, model training, evaluation, and deployment through an interactive Streamlit dashboard.

## 🚀 Introduction

Credit risk assessment plays an important role in banking and financial institutions. Before approving a loan, lenders need to evaluate whether an applicant is likely to repay the borrowed amount.

This project uses machine learning classification algorithms to predict loan default risk based on historical financial data.

The application provides an interactive dashboard where users can enter applicant details, generate predictions, analyze model performance, and explore important factors influencing credit risk.

## ✨ Key Features

- Data Cleaning and Missing Value Imputation
- Feature Engineering and Categorical Encoding
- Exploratory Data Analysis (EDA)
- Multiple Machine Learning Models
- Model Accuracy Comparison
- Confusion Matrix Evaluation
- Feature Importance Analysis
- Real-Time Credit Risk Prediction
- Risk Classification (Low / Medium / High)
- Interactive Streamlit Dashboard
- Automated PDF Report Generation
- Model Persistence using Joblib
- Dataset Overview with Interactive Charts

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Data Processing | Pandas, NumPy |
| Machine Learning | Scikit-learn |
| Data Visualization | Matplotlib, Seaborn, Plotly |
| Web Framework | Streamlit |
| Model Persistence | Joblib |
| PDF Generation | ReportLab |
| Development Tools | Jupyter Notebook, Git, GitHub |

## 📊 Dataset

The project uses a credit risk dataset containing **32,581 loan applicant records** with 12 columns (11 input features and 1 target variable).

**Dataset Details:**

- Total Records: 32,581
- Total Features: 11
- Target Column: `loan_status`
- 0 = No Default
- 1 = Default
- No Default: 78.2%
- Default: 21.8%

**Features Used:**

- `person_age`
- `person_income`
- `person_home_ownership`
- `person_emp_length`
- `loan_intent`
- `loan_grade`
- `loan_amnt`
- `loan_int_rate`
- `loan_percent_income`
- `cb_person_default_on_file`
- `cb_person_cred_hist_length`

**Data Preprocessing:**

- Handled missing values using median imputation.
- Applied Label Encoding to categorical variables.
- Used binary mapping for previous default history.
- Applied One-Hot Encoding to loan intent and loan grade.
- Prepared the dataset for machine learning model training.

## 🔍 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the dataset and identify patterns related to loan defaults.

Key analysis included:

- Class Distribution Analysis
- Missing Value Analysis
- Feature Distribution Analysis
- Correlation Heatmap
- Loan Grade Analysis
- Relationship Between Income and Loan Amount

These visualizations helped identify important patterns and relationships between applicant characteristics and loan default risk.

## 🤖 Machine Learning Models

Three classification algorithms were trained and compared:

| Model | Accuracy |
|---|---:|
| Logistic Regression | 83.12% |
| Decision Tree Classifier | 89.09% |
| Random Forest Classifier | 93.34% |

<badge color="success">Best notebook accuracy: 93.34%</badge>

The Random Forest Classifier achieved the highest accuracy among the three models.

## 🔄 Machine Learning Workflow

1. Data Collection
2. Data Cleaning
3. Exploratory Data Analysis
4. Feature Engineering
5. Categorical Encoding
6. Train-Test Split (80/20)
7. Model Training
8. Model Evaluation
9. Model Saving
10. Streamlit Deployment

## 📈 Model Evaluation

Model performance was evaluated using:

- Accuracy Score
- Confusion Matrix
- Model Comparison

The notebook's saved results include accuracy scores and a confusion matrix. Other evaluation metrics, such as precision, recall, F1-score, and ROC-AUC, are not included in the reported results.

## 🔬 Feature Importance

Feature importance analysis helps understand which variables contribute most to credit risk predictions.

Important factors identified include:

- Loan Grade
- Loan-to-Income Ratio
- Interest Rate

These features provide useful insights into the factors influencing loan default predictions.

## 📂 Project Structure

```text
credit-scoring-system/
│
├── README.md
│
└── Credit_Scoring_System/
    │
    ├── app.py
    ├── credit_score_model.ipynb
    ├── requirements.txt
    │
    ├── dataset/
    │   └── credit_risk_dataset.csv
    │
    ├── model/
    │   └── credit_score.pkl
    │
    └── images/
        ├── dataset_overview.png
        ├── distribution.png
        ├── heatmap.png
        ├── confusion_matrix.png
        ├── feature_insights.png
        ├── gui1.png
        ├── model_analytics.png
        ├── prdiction_page.png
        └── dashboard_preview.gif
```



## 📘 Application Usage

The Streamlit dashboard contains four main sections:

**1. Prediction**
- Enter applicant and loan information.
- Select a machine learning model.
- Generate credit risk predictions.
- View predicted outcomes and risk levels.
- Download PDF prediction reports.

**2. Model Analytics**
- Compare model accuracy.
- Analyze model performance.
- View the confusion matrix.

**3. Feature Insights**
- Explore feature importance.
- Analyze default rates across loan grades.
- Understand important factors influencing predictions.

**4. Dataset Overview**
- View dataset statistics.
- Explore loan-purpose distributions.
- Analyze sample records and visualizations.

## ⚠️ Important Implementation Notes

- The notebook reports Random Forest as the best-performing model with 93.34% accuracy.
- The currently saved model artifact (`credit_score.pkl`) is a Decision Tree model with 89.09% accuracy, rather than the best-performing Random Forest.
- The deployed demonstration application uses a 3,000-row synthetic dataset for responsive model demonstrations.
- Displayed accuracy values are based on the original notebook results, while some live evaluation outputs reflect the synthetic dataset.

Therefore, the deployed application should be treated as a demonstration rather than a production-ready credit approval system.

## 🔮 Future Improvements

- Deploy the best-performing Random Forest model.
- Add precision, recall, F1-score, and ROC-AUC evaluation.
- Implement feature scaling for Logistic Regression.
- Perform hyperparameter tuning using GridSearchCV or Optuna.
- Integrate SHAP for explainable AI.
- Develop a REST API for model predictions.
- Implement Docker containerization.
- Add automated model monitoring and retraining.
- Implement CI/CD pipelines.
- Explore cloud deployment options.

## 📜 License

This project is intended for educational, learning, and portfolio purposes. Review and retain the original repository's license and required attribution notices when redistributing or modifying the project.

## 👨‍💻 Author

Abhay Singh

---

⭐ If you find this project useful, consider giving the repository a star!
