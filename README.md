# Game_churn_prediction
**Game Churn Prediction Project**

**Project Overview**
This project focuses on predicting whether a player will stop playing a game (churn) based on behavioral, demographic, and engagement-related features. The goal is to help game companies identify at-risk users and improve retention strategies using machine learning.

**Dataset Description**
The dataset contains player-level information such as:
Demographics:
Age
Gender
Location
Game Behavior:
Game Genre
Game Difficulty
Play Time (hours)
Sessions per week
Average session duration
Player level
Achievements unlocked
In-game purchases
Engagement Features:
Engagement level (Low / Medium / High)
Churn status (Target variable)

**Workflow**

1. Data Preprocessing
Handled missing values and cleaned dataset
Converted categorical variables using encoding techniques
Standardized numerical features using StandardScaler
2. Exploratory Data Analysis (EDA)
Analyzed churn distribution and class imbalance
Visualized relationships between churn and:
Gender
Game genre
Engagement level
Playtime and activity metrics
Identified key behavioral patterns affecting churn
3. Feature Engineering
Created new features:
Engagement Score = Sessions per week × Avg session duration
Achievements per Level = Achievements unlocked / Player level
Checked multicollinearity using VIF (Variance Inflation Factor)
4. Encoding
Label encoding for ordinal features (e.g., difficulty, engagement level)
One-hot encoding for categorical variables like:
Location
Game genre
5. Model Building

Trained multiple classification models:

Logistic Regression
K-Nearest Neighbors (KNN)
Decision Tree
Random Forest
Extra Trees Classifier
Gradient Boosting
6. Model Evaluation

Each model was evaluated using:

Accuracy
Precision
Recall
F1 Score
ROC-AUC Score
Stratified 5-Fold Cross Validation

Also included:

Confusion matrix visualization
ROC curve comparison
7. Model Selection

Models were compared based on ROC-AUC and stability across cross-validation. Ensemble models performed better than basic classifiers.

8. Feature Importance Analysis

Feature importance was extracted from tree-based models (Random Forest, Gradient Boosting, Extra Trees) to identify key drivers of churn.

**Tech Stack**
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
Statsmodels
**Conclusion**
This project demonstrates a complete machine learning pipeline from data preprocessing to model evaluation and business insight generation, focused on improving player retention in gaming platforms.
