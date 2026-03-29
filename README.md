# Syntecxhub_Salary_Prediction

## 💼 Salary Prediction (Linear Regression)
This project is part of my Machine Learning internship at Syntecxhub (Task-01). It demonstrates a regression-based approach to predict salary based on experience and additional features.

## 📌 Objective
Build a regression model to predict salary using:

1. Experience
2. Test Score (synthetically added for demonstration of multiple regression)
3. Salary

The project compares single-feature and multi-feature linear regression models and evaluates their performance.

## ⚙️ Workflow
1. Loaded dataset (Salary_dataset.csv) using pandas
2. Explored dataset structure and summary statistics
3. Visualized relationship between experience and salary
4. Defined features and target variable
5. Performed train-test split using scikit-learn
6. Trained a Linear Regression model using a single feature
7. Evaluated model using RMSE and R² score
8. Created a synthetic feature (Test Score) to demonstrate multiple regression
9. Trained a second Linear Regression model with multiple features
10. Compared both models based on evaluation metrics
11. Selected the best model and saved it using joblib
12. Generated predictions and compared them with actual values

## 📊 Results
1. Single Feature Model:
   - RMSE: 7059.04362190151
   - R² Score: 0.9024461774180497

3. Multiple Feature Model:
   - RMSE: 5.94e-12
   - R² Score: 1.0

👉 Note: The multiple feature model achieved perfect performance due to data leakage, as one of the features was derived from the target variable.

## 📂 Dataset
The dataset ([Salary_dataset.csv](https://www.kaggle.com/datasets/abhishek14398/salary-dataset-simple-linear-regression/data)) contains:
- YearsExperience
- Salary

Additionally, a synthetic feature (TestScore) was created for demonstration purposes to simulate multiple regression. The dataset is included in this repository.

## 📈 My Prediction
Predicted Salary: 71499.2780946286

## 🚀 Tech Stack
1. Python
2. Pandas
3. NumPy
4. Scikit-learn
5. Matplotlib
6. Joblib

## ▶️ How to Run
pip install -r requirements.txt </br>
jupyter notebook

## 💡 Note
- This project demonstrates the full machine learning workflow for regression tasks.
- The multiple regression model shows perfect performance due to the inclusion of a synthetic feature derived from the target variable.
- In real-world scenarios, all features should be independent of the target variable to avoid data leakage.
- Further improvements can be made by using real multi-feature datasets and advanced regression techniques.
