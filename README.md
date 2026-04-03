# ⚽ Player Value Prediction
📖 Overview

This project focuses on predicting the market value of football players using machine learning techniques. By analyzing player attributes such as age, technical skills, and club information, the model estimates a player’s value and identifies key factors influencing it.

🎯 Objective
Predict player market value (regression task)
Understand the impact of player attributes on valuation
Build an optimized machine learning model using tuning techniques
📊 Dataset

The dataset contains player-level information including:

Age and demographics
Club and country
Technical attributes (reactions, ball control, composure, etc.)
Market value (target variable)
⚙️ Methodology
Data Preprocessing
Removed unnecessary identifier column (player)
Cleaned the value column (removed symbols and formatting)
Dropped columns with all missing values (e.g., marking)
Removed duplicate records
Encoded categorical features (country, club) using Label Encoding
Exploratory Data Analysis
Distribution analysis of features such as age and reactions
Relationship analysis between:
Age and player value
Reactions and player value
Ball control and player value
Correlation heatmap to identify important features
Feature Engineering
Outlier removal using the IQR method
Feature scaling using StandardScaler
Dimensionality reduction using PCA (25 components)
Model Development
Baseline Model: RandomForestRegressor
Optimized Model: RandomForestRegressor with GridSearchCV

Hyperparameters tuned:

Number of estimators
Maximum depth
Minimum samples split
📈 Model Performance
Metric	Value
MAE	385,495
MSE	323,230,920,490
RMSE	568,534
R² Score	0.62
🔍 Key Insights
Player value peaks in the mid-20s age range
Higher reaction scores strongly increase player value
Technical skills such as ball control and composure are major contributors
Goalkeeper-specific attributes have lower impact on overall valuation
🚀 Future Improvements
Use advanced models like XGBoost or LightGBM
Apply log transformation on the target variable
Include additional features such as player position and performance stats
Deploy the model using Streamlit or Flask
▶️ How to Run
git clone https://github.com/your-username/player-value-prediction.git
cd player-value-prediction
pip install -r requirements.txt

Run the notebook or script to train the model.

📌 Conclusion

This project demonstrates a complete machine learning pipeline for predicting player value. The model achieves a reasonable performance and provides meaningful insights that can support decision-making in player scouting and transfers.
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
