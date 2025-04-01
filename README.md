# House Price Prediction using Machine Learning

## Overview
This project implements a Machine Learning model to predict house prices based on various features such as area, number of bedrooms, bathrooms, stories, parking, and other factors. The dataset used for training and evaluation contains multiple attributes related to housing.

## Dataset
The dataset (`Housing.csv`) consists of 545 records with the following features:
- `price` (target variable)
- `area`
- `bedrooms`
- `bathrooms`
- `stories`
- `mainroad`
- `guestroom`
- `basement`
- `hotwaterheating`
- `airconditioning`
- `parking`
- `prefarea`
- `furnishingstatus`

## Steps Involved
1. **Load the dataset**: The dataset is read using Pandas.
2. **Preprocessing**:
   - Handle missing values (if any).
   - Normalize numerical features using MinMaxScaler.
   - Convert categorical variables to numerical values (if necessary).
3. **Train-Test Split**: The data is split into training and testing sets (80-20 ratio).
4. **Model Training**: A Linear Regression model is trained on the dataset.
5. **Prediction & Evaluation**:
   - Predictions are made using the trained model.
   - Evaluation metrics used:
     - Mean Squared Error (MSE)
     - R-squared Score (R²)
   - A scatter plot is generated to visualize actual vs predicted prices.

## Code Execution
Run the Python script using:
```bash
python house_price_prediction.py
```

## Results
- **Mean Squared Error (MSE)**: 0.0172
- **R-squared Score (R²)**: 0.5464

## Visualization
The scatter plot below represents the actual vs predicted prices:

![Actual vs Predicted Prices](plot.png)  

## Future Improvements
- Feature engineering to include additional relevant variables.
- Hyperparameter tuning for better model accuracy.
- Trying other regression models (Decision Trees, Random Forest, etc.).
