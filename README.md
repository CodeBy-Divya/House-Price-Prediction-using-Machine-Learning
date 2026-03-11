
# 🏠 Boston House Price Prediction using XGBoost

This project builds a **Machine Learning Regression Model** to predict house prices using the **Boston Housing Dataset**. The model is trained using **XGBoost Regressor**, and performance is evaluated using **R² Score** and **Mean Absolute Error (MAE)**.

---

# 📌 Project Overview

The goal of this project is to predict housing prices based on several features such as:

* Crime rate
* Number of rooms
* Property tax rate
* Distance to employment centers
* Percentage of lower status population
* And more housing-related factors

We use **XGBoost Regression**, a powerful gradient boosting algorithm widely used for structured data.

---

# ⚙️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost

---

# 📂 Dataset

The dataset used is the **Boston Housing Dataset**, available in `sklearn.datasets`.

It contains **506 rows and 13 features** related to housing attributes.

### Features include:

| Feature | Description                          |
| ------- | ------------------------------------ |
| CRIM    | Crime rate per town                  |
| ZN      | Proportion of residential land zoned |
| INDUS   | Non-retail business acres            |
| CHAS    | Charles River dummy variable         |
| NOX     | Nitric oxide concentration           |
| RM      | Average number of rooms              |
| AGE     | Proportion of old houses             |
| DIS     | Distance to employment centers       |
| RAD     | Accessibility to highways            |
| TAX     | Property tax rate                    |
| PTRATIO | Pupil-teacher ratio                  |
| B       | Proportion of Black population       |
| LSTAT   | % lower status population            |

**Target Variable**

* `price` → Median value of owner-occupied homes.

---

# 🔎 Project Workflow

### 1️⃣ Import Dependencies

Libraries such as NumPy, Pandas, Seaborn, Matplotlib, and Scikit-learn are imported.

### 2️⃣ Load Dataset

The Boston Housing dataset is loaded from `sklearn.datasets`.

### 3️⃣ Data Exploration

* View first 5 rows
* Check dataset shape
* Check missing values
* Statistical summary

### 4️⃣ Correlation Analysis

A **heatmap** is created using Seaborn to visualize correlations between features.

### 5️⃣ Data Splitting

Dataset is split into:

* **80% Training Data**
* **20% Testing Data**

Using `train_test_split()`.

### 6️⃣ Model Training

The **XGBoost Regressor** is used to train the model.

```
model = XGBRegressor()
model.fit(X_train, Y_train)
```

### 7️⃣ Model Evaluation

Two evaluation metrics are used:

* **R² Score**
* **Mean Absolute Error (MAE)**

### 8️⃣ Visualization

A scatter plot compares:

* **Actual Prices**
* **Predicted Prices**

---

# 📊 Model Performance

### Training Data

* **R² Score** → Measures how well predictions match actual values
* **Mean Absolute Error** → Average prediction error

### Test Data

Performance is also evaluated on unseen test data to check generalization.

---

# 📈 Visualization

Scatter Plot:

* X-axis → Actual House Prices
* Y-axis → Predicted House Prices

If the model performs well, points will lie close to the **diagonal line**.

---

# 🚀 How to Run the Project

### 1️⃣ Clone the Repository

```
git clone https://github.com/your-username/boston-house-price-prediction.git
```

### 2️⃣ Install Dependencies

```
pip install numpy pandas matplotlib seaborn scikit-learn xgboost
```

### 3️⃣ Run the Script

```
python house_price_prediction.py
```

---

# 📌 Future Improvements

Possible improvements include:

* Hyperparameter tuning
* Feature engineering
* Cross-validation
* Model comparison (Random Forest, Linear Regression)
* Deploying the model using Flask or FastAPI

---

# 👨‍💻 Author

**Divya Singh**

Machine Learning Enthusiast | Data Science Learner


