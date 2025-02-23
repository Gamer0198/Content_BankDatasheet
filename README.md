# Banking Data Analysis & Prediction

## Overview
This project analyzes banking data to predict the success of a marketing campaign using **Logistic Regression**. The dataset includes customer demographics, financial information, and previous campaign outcomes. The goal is to predict whether a customer will respond positively to the campaign using various **machine learning techniques** and **data visualization**.

## Dataset
The dataset contains information on:
* **Customer Demographics**: Age, marital status, education, job type
* **Financial Details**: Balance, loan status, housing loan status
* **Campaign Features**: Duration, number of previous contacts, and outcome of past campaigns

## Project Workflow

### 1. Data Cleaning & Preprocessing
* Handle missing values
* Convert categorical variables using **One-Hot Encoding** & **Ordinal Encoding**
* Standardize numerical features using **StandardScaler**

### 2. Feature Engineering
* Create new features (e.g., `success_rate` based on previous campaign outcomes)

### 3. Train-Test Split
* Split data into 80% training and 20% testing

### 4. Model Training & Evaluation
* Train a **Logistic Regression Model**
* Evaluate using **Accuracy, Precision, Recall, and F1-Score**

### 5. Data Visualization
* Heatmaps, bar plots, and pie charts to explore feature relationships

## Technologies Used
* **Python**
* **Pandas, NumPy** for data manipulation
* **Matplotlib, Seaborn** for data visualization
* **Scikit-learn** for machine learning and evaluation

## Model Performance

| Metric | Score |
|--------|-------|
| **Accuracy** | 96.36% |
| **Precision** | 97% (Class 0), 9% (Class 1) |
| **Recall** | 100% (Class 0), 1% (Class 1) |
| **F1 Score** | 98% (Class 0), 2% (Class 1) |

### Confusion Matrix
```
[[8710   29]
 [ 300    3]]
```
* **Class 0 (Not Subscribed)**: Well predicted
* **Class 1 (Subscribed)**: Needs improvement (high imbalance)

## Visualization
* 📊 **Feature Correlation Heatmap**
* 📈 **Marital Status, Education, and Campaign Outcome Distributions**
* 🥧 **Loan and Housing Loan Pie Charts**

## Installation & Usage

### 1. Clone Repository
```bash
git clone https://github.com/yourusername/banking-data-analysis.git
cd banking-data-analysis
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the Script
```bash
python banking_analysis.py
```

## Future Improvements
* **Handling Imbalanced Data**: Use **SMOTE (Synthetic Minority Over-sampling Technique)**
* **Try Advanced Models**: Random Forest, XGBoost, or Neural Networks
* **Hyperparameter Tuning**: GridSearchCV for better optimization

## Contributors
* **Anant Sinha**

## License
This project is licensed under the **MIT License**.
