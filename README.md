# ⚽ Player Value Prediction using FIFA Dataset

## 📖 Overview
This project focuses on predicting the **market value of football players** using machine learning techniques. It analyzes player attributes such as physical characteristics, technical skills, and performance metrics to estimate their value.

The project also evaluates:
- Dimensionality Reduction (PCA)
- Hyperparameter Tuning (GridSearchCV)

---

## 🎯 Objective
- Predict player market value (regression problem)
- Identify key factors influencing player value
- Compare model performance:
  - Baseline vs Tuned model
  - PCA vs Non-PCA

---

## 📊 Dataset
The dataset contains player-level information including:
- Player details (country, club)
- Physical attributes (age, height, weight)
- Technical skills (ball control, reactions, passing, etc.)
- Performance metrics
- Market value (target variable)

---

## ⚙️ Project Workflow

### 1. Data Loading
- Loaded dataset from CSV file

### 2. Data Understanding
- Checked structure, data types, and summary statistics
- Identified numerical and categorical features

### 3. Data Cleaning
- Removed identifier column (player)
- Cleaned target variable (removed symbols)
- Dropped columns with all null values
- Removed duplicate records

### 4. Feature Engineering
- Encoded categorical variables (country, club)
- Removed outliers using IQR method
- Standardized features using scaling

### 5. Exploratory Data Analysis (EDA)
- Performed univariate analysis (feature distribution)
- Performed bivariate analysis (feature vs value)
- Generated correlation heatmap

### 6. Dimensionality Reduction (PCA)
- Applied PCA to reduce feature dimensions
- Selected components explaining 95% variance

### 7. Model Building

#### Baseline Model
- Random Forest Regressor

#### Optimized Model
- Random Forest with GridSearchCV

### 8. Model Evaluation
Models evaluated using:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## 📈 Results
- R² Score: ~0.62
- RMSE: ~568,000
- Tuned model performed better than baseline

---

## 🔍 Key Insights
- Player value peaks in mid-20s
- Technical skills (reactions, ball control, composure) strongly influence value
- Some features (goalkeeper attributes) have lower impact
- High-value players create skewed distribution

---

## 🚀 Future Improvements
- Use advanced models (XGBoost, LightGBM)
- Apply log transformation on target variable
- Add more features (goals, assists, position)
- Deploy model using Streamlit or Flask

---

## ▶️ How to Run

```bash
git clone https://github.com/your-username/player-value-prediction.git
cd player-value-prediction
pip install -r requirements.txt
```

Run the notebook to train and evaluate the model.

---

## 📌 Conclusion
This project demonstrates a complete machine learning pipeline for predicting player value. It highlights the importance of feature engineering, dimensionality reduction, and hyperparameter tuning in improving model performance.

---

## 👨‍💻 Author
Aniket Sawant
