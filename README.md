#⚽ Player Value Prediction
📖 Overview

This project aims to predict the market value of football players using machine learning techniques. The model analyzes player attributes such as age, technical skills, and club information to estimate their value and identify key influencing factors.

🎯 Objective
Predict player market value (regression problem)
Identify important features affecting player value
Build and optimize a machine learning model
📊 Dataset

The dataset contains player-level information, including:

Demographic details (age, country)
Club information
Technical attributes (reactions, ball control, composure, etc.)
Market value (target variable)
⚙️ Project Workflow
1. Data Loading
Imported dataset from CSV file
Loaded data into a structured format for analysis
2. Data Understanding
Checked dataset shape, structure, and data types
Reviewed summary statistics
Identified numerical and categorical features
3. Data Cleaning
Removed unnecessary identifier column (player name)
Cleaned the target variable by removing symbols
Dropped columns with all missing values
Verified and ensured no remaining null values
Removed duplicate records
4. Feature Classification
Divided dataset into:
Categorical features (country, club)
Numerical features (age, technical stats)
5. Data Transformation
Converted categorical features into numerical form using encoding
Prepared dataset for machine learning algorithms
6. Outlier Handling
Detected outliers using the IQR method
Removed extreme values to improve model performance
7. Exploratory Data Analysis (EDA)
Univariate Analysis
Analyzed distribution of features like age and reactions
Bivariate Analysis
Studied relationships between:
Age and player value
Reactions and player value
Ball control and player value
Correlation Analysis
Identified strong and weak relationships between features
8. Feature Scaling
Standardized numerical features to bring them to the same scale
9. Dimensionality Reduction (PCA)
Applied PCA to reduce feature dimensions
Retained important components capturing most variance
10. Data Splitting
Divided dataset into training and testing sets
Used training data for model learning and testing data for evaluation
11. Model Building
Baseline Model
Built initial model using Random Forest Regressor
Optimized Model
Improved model using hyperparameter tuning (GridSearchCV)
12. Model Evaluation
Evaluated model performance using:
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R² Score
13. Key Insights
Player value peaks around mid-20s
Higher reaction scores increase player value
Technical attributes strongly influence value
Some features contribute more significantly than others
14. Conclusion
Successfully built a machine learning model to predict player value
Identified important factors affecting player valuation
Provided insights useful for decision-making in sports analytics
