# ⚽ Player Value Prediction using Machine Learning
It is the player value prediction model build with the Gridsearchcv

📌 Project Overview

This project aims to predict the market value of football players using machine learning techniques. It uses player statistics such as age, reactions, ball control, and other attributes to estimate their value.

The project follows a complete ML pipeline including:

Data Cleaning
Exploratory Data Analysis (EDA)
Feature Engineering
Dimensionality Reduction (PCA)
Model Building (Random Forest)
Hyperparameter Tuning (GridSearchCV)
🎯 Objective
Predict player market value (Regression Problem)
Identify key features affecting player value
Improve prediction accuracy using tuning techniques
📂 Dataset
File: player_stats.csv
Contains player attributes such as:
Age
Country
Club
Technical skills (reactions, ball control, etc.)
Market value (target variable)
🧪 Technologies Used
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
🔍 Project Workflow
1. Data Preprocessing
Removed unnecessary columns (player)
Cleaned target column (value)
Removed null columns (marking)
Removed duplicate records
Label Encoding for categorical variables (country, club)
2. Exploratory Data Analysis (EDA)
Univariate Analysis:
Age distribution
Reactions distribution
Bivariate Analysis:
Age vs Value
Reactions vs Value
Ball Control vs Value
Correlation Heatmap used to identify relationships
3. Feature Engineering
Outlier removal using IQR method
Feature scaling using StandardScaler
Dimensionality reduction using PCA (25 components)
4. Model Building
✅ Baseline Model
Algorithm: RandomForestRegressor
✅ Optimized Model
Used GridSearchCV for hyperparameter tuning
param_grid = {
    'n_estimators': [50, 100, 150],
    'max_depth': [None, 5, 10],
    'min_samples_split': [2, 5, 10]
}
5. Model Evaluation
Metrics Used:
MAE (Mean Absolute Error)
MSE (Mean Squared Error)
RMSE (Root Mean Squared Error)
R² Score
📊 Final Results:
MAE: 385,495
MSE: 323,230,920,490
RMSE: 568,534
R² Score: 0.62
📈 Key Insights
Player value peaks in mid-20s age range
Higher reactions → higher value
Better ball control → higher value
Technical attributes strongly influence player price
Goalkeeper attributes have less impact on overall value
🚀 Improvements Applied
PCA for dimensionality reduction
GridSearchCV for hyperparameter tuning
Outlier removal for better model performance
🔮 Future Improvements
Use advanced models like:
XGBoost
LightGBM
Apply log transformation on target variable
Add more features like:
Goals, assists
Player position
Deploy using:
Streamlit
Flask API
🛠️ How to Run the Project
# Step 1: Clone the repository
git clone https://github.com/your-username/player-value-prediction.git

# Step 2: Navigate to project folder
cd player-value-prediction

# Step 3: Install dependencies
pip install -r requirements.txt

# Step 4: Run the notebook/script
📌 Conclusion
Built a machine learning model to predict player value
Achieved R² score of 0.62 using RandomForestRegressor
Identified key factors affecting player valuation
Project demonstrates complete ML workflow from data to insights
