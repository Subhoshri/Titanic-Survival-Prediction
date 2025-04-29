# Titanic Survival Prediction

This project predicts which passengers survived the Titanic shipwreck using supervised machine learning. It’s a classic binary classification task based on real-world data from Kaggle.

---

## Objective

Predict the `Survived` label (0 or 1) using features such as passenger class, sex, age, fare, and more. This serves as a foundational ML project for learning data preprocessing, model building, and evaluation.

## Dataset

- Source: [Kaggle Titanic Dataset](https://www.kaggle.com/competitions/titanic/data)
- Files used:  
  - `train.csv` – training data  
  - `test.csv` – test data for prediction  

## Workflow

1. **Data Cleaning & Preprocessing**
   - Handled missing values (`Age`, `Embarked`)
   - Dropped features with high missingness (`Cabin`)
   - Encoded categorical variables (`Sex`, `Embarked`) using One-Hot Encoding
   - Converted `Pclass` into ordinal numerical values

2. **Exploratory Data Analysis**
   - Visualized survival rates by `Sex`, `Age`, `Pclass`, `Fare`
   - Correlation heatmap for feature relationships

3. **Model Building**
   - Evaluated accuracy of base models using Logistic Regression, Decision Tree, Random Forest Classifier, Support Vector Classifier and XGBoost Classifier
   - Hypertuned Random Forest Classifier, SVC and XGBoost Classifier for improved accuracy

4. **Model Evaluation**
   - Used Accuracy, Precision, Recall, F1 Score
   - Applied `train_test_split` with 80-20 ratio
  
5. **Results**
   - Achieved accuracy score of 84.35% with Random Forest Classifier.
   - Predicted survival rates of test.csv

## Models & Performance

| Model                     | Accuracy | F1 Score |
|---------------------------|----------|----------|
| Support Vector Classifier | 82%      |  0.75    |
| Random Forest Classifier  | 84%      |  0.79    |
| XGBoost Classifier        | 83%      |  0.77    |

## Learnings

- Learned essential preprocessing steps and encoding
- Understood how feature selection impacts accuracy
- Discovered that ensemble models like Random Forest perform better on structured data
- Practiced model evaluation and tuning basics

## Note

This project was done for learning purposes and is part of my ML practice roadmap.
