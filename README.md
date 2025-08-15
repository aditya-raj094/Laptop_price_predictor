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
   - Extracted processor details from the `Cpu` column

3. **Feature Engineering**  
   - Removed unnecessary text from features  
   - Created indicators for **Touchscreen** and **IPS**  
   - Ensured price values are numerical

4. **Model Building & Evaluation**  
   - Split data into **Train (85%)** and **Test (15%)**  
   - Evaluated multiple models:  
     - Linear Regression  
     - Ridge Regression  
     - Lasso Regression  
     - K-Nearest Neighbors (KNN)  
     - Decision Tree Regressor  
     - Support Vector Regression (SVR)
     - Random Forest Regressor  
     - Gradient Boosting Regressor  
     - AdaBoost Regressor

---

## 🏆 Best Model

- **Random Forest Regression**
  - **R² (Test)**: *Highest among all models*
  - **MAE (Test)**: *Lowest among all models*

---

## 📈 Model Performance Results

Evaluation metrics: **R² Score** (coefficient of determination) and **MAE** (Mean Absolute Error).

| Model                         | R² Score | MAE     |
|------------------------------|----------|---------|
| Linear Regression            | 0.8073   | 0.2102  |
| Ridge Regression             | 0.8127   | 0.2093  |
| Lasso Regression             | 0.8072   | 0.2111  |
| K-Nearest Neighbors (KNN)    | 0.8031   | 0.1926  |
| Decision Tree                | 0.8415   | 0.1816  |
| Support Vector Regression    | 0.8083   | 0.2024  |
| **Random Forest**            | ✅ 0.8873 | 0.1586  |
| Gradient Boosting            | 0.8806   | 0.1600  |
| AdaBoost                     | 0.7933   | 0.2303  |

---

### 🔹 Key Observations
- **Random Forest** delivers the best performance with the highest R² and lowest MAE.  
- **Gradient Boosting** is a close second on R² and MAE.  
- Linear baselines (Linear/Lasso/Ridge) perform reasonably well; **SVM** and **KNN** add competitive non-linear baselines.


