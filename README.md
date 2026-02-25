TTitanic Survival Prediction using Random Forest 🚢
This repository contains a Machine Learning project developed to predict the survival status of passengers on the Titanic using the classic Kaggle dataset. The project focuses on feature engineering, model optimization, and performance evaluation metrics such as Precision, Recall, and F1-Score.

📌 Project Overview
The goal is to build a classification model that predicts whether a passenger survived based on features like age, sex, passenger class, and family size.

🛠️ Tech Stack
Language: Python 3.9

Libraries: Pandas, NumPy, Scikit-Learn, Matplotlib

Environment: Anaconda / Jupyter Notebook

📊 Model Performance
After hyperparameter tuning (n_estimators=200, max_depth=8), the model achieved a significant improvement in capturing survivors (Recall).

Final Metrics:
| Metric | Class 0 (Not Survived) | Class 1 (Survived) | Combined (Accuracy) |
| :--- | :---: | :---: | :---: |
| Precision | 0.82 | 0.85 | - |
| Recall | 0.91 | 0.72 | - |
| F1-Score | 0.86 | 0.78 | 0.83 |

Confusion Matrix Insights
Plaintext
[[96  9]  <- Predicted 96 correct negatives, 9 false positives
 [21 53]] <- Predicted 53 correct positives, 21 false negatives
🚀 Key Insights & Improvements
Hyperparameter Tuning: Increased n_estimators to 200 and set max_depth to 8, which improved the Recall of the "Survived" class from 0.68 to 0.72.

Feature Importance: Analyzed the decision-making process of the Random Forest; Sex and Pclass were the most influential features in predicting survival.

Data Preprocessing: Handled missing values in the 'Age' column using mean imputation and performed label encoding for categorical variables.
