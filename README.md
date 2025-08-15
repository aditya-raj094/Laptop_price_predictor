# 💻 Laptop Price Prediction

This project predicts laptop prices using machine learning models. It uses the **`laptop_data`** dataset from Kaggle and evaluates multiple algorithms, with **Random Forest Regression** achieving the best R² score.

---

## 📂 Dataset

- **Source**: [Laptop Price Prediction Dataset (Kaggle)]
- **File Used**: `laptop_data.csv`
- **Features**:
  - Company, TypeName, Inches, ScreenResolution, Cpu, Ram, Memory, Gpu, OpSys, Weight
- **Target Variable**:
  - Price 

---

## 🛠️ Technologies Used

- **Python**
- **Pandas** – Data handling
- **NumPy** – Numerical computations
- **Matplotlib & Seaborn** – Visualization
- **Scikit-learn** – Machine learning models
- **Jupyter Notebook** – Development

---

## 📊 Steps Followed

1. **Data Loading & Exploration**  
   - Loaded CSV data using Pandas  
   - Checked for null values and data types  
   - Performed descriptive statistics

2. **Data Preprocessing**  
   - Handled categorical variables with **One-Hot Encoding**  
   - Converted RAM, Weight, and Memory columns to numeric values  
   - Extracted processor details from `Cpu` column

3. **Feature Engineering**  
   - Removed unnecessary text from features  
   - Created new features like touch screen & IPS indicator  
   - Converted all prices to numerical format

4. **Model Building & Evaluation**  
   - Split data into **Train (85%)** and **Test (15%)**  
   - Tried multiple models:  
     - Linear Regression  
     - Lasso Regression  
     - Ridge Regression  
     - K-Nearest Neighbors (KNN)  
     - Decision Tree Regressor  
     - Random Forest Regressor  
     - Gradient Boosting Regressor  
     - AdaBoost Regressor  
     - XGBoost Regressor  

---

## 🏆 Best Model

- **Random Forest Regression**
  - **R² Score (Test)**: *Highest among all models*
  - **Mean Absolute Error**: *Lowest among all models*

---

##  📈 Model Performance Result

The table below summarizes the performance of different regression models applied to our dataset. The evaluation metrics used are **R² Score** (coefficient of determination) and **MAE** (Mean Absolute Error).  

| Model                        | R² Score | MAE     |
|-------------------------------|----------|---------|
| Linear Regression             | 0.8073   | 0.2102  |
| Lasso Regression              | 0.8127   | 0.2093  |
| Ridge Regression              | 0.8072   | 0.2111  |
| K-Nearest Neighbors (KNN)     | 0.8031   | 0.1926  |
| Decision Tree                 | 0.8415   | 0.1816  |
| Random Forest                 | ✅ 0.8873 | 0.1586  |
| Gradient Boosting             | 0.7933   | 0.2303  |
| AdaBoost                      | 0.8806   | 0.1600  |
| XGBoost                       | 0.8083   | 0.2024  |

### 🔹 Key Observations
- **Random Forest** achieved the highest R² score and the lowest MAE, making it the **best-performing model** for this dataset.  
- **Decision Tree** and **AdaBoost** also performed well, with reasonably high R² and low MAE.  
- Linear models like **Linear Regression, Lasso, and Ridge** provided good baseline performance but were slightly less accurate than ensemble methods.

