# EL_Task3
# 🏠 Housing Price Prediction

This project uses **Linear Regression** to predict housing prices based on various features such as area, number of bedrooms, bathrooms, furnishing status, and more.

## 📁 Dataset

The dataset used is `Housing.csv`, which contains the following features:

- `price` (target)
- `area`, `bedrooms`, `bathrooms`, `stories`, `parking`
- `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `prefarea`, `furnishingstatus` (categorical)

## 📊 Project Workflow

1. **Import and Preprocess Data**
    - Load the dataset using `pandas`
    - Handle categorical features with one-hot encoding
    - Check for missing values

2. **Split Dataset**
    - Use `train_test_split()` to split data into training and testing sets (80/20)

3. **Train Model**
    - Use `sklearn.linear_model.LinearRegression` to fit the model

4. **Evaluate Model**
    - Metrics used:
        - MAE (Mean Absolute Error)
        - MSE (Mean Squared Error)
        - R² Score

5. **Visualize Results**
    - Plot regression line of area vs price using `matplotlib` and `seaborn`
    - Interpret model coefficients


## 🧠 Interpretation

- Features like `bathrooms`, `airconditioning`, and `hotwaterheating` have a strong positive effect on price.
- Unfurnished homes lower the price significantly.
- The model explains approximately 49% of the variation in price using the available features.

## 🛠️ Technologies Used

- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
