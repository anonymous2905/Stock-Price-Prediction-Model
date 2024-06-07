# Stock Price Prediction Project

## Overview
This project aims to predict stock prices for large-cap, mid-cap, and small-cap companies. The project involves several stages including data collection, preprocessing, model training, evaluation, and selection of the best-performing model based on Mean Squared Error (MSE).

## Project Structure
- `data/`: Contains CSV files for large-cap, mid-cap, and small-cap stock data.
- `notebooks/`: Contains the Jupyter Notebook `stock_price_model_prediction.ipynb` for model training and evaluation.
- `models/`: Directory for storing trained models.

## Setup Instructions
1. Clone the repository:
    ```bash
    git clone https://github.com/anonymous2905/stock-price-prediction.git
    cd stock-price-prediction
    ```
2. Install required packages:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter Notebook:
    ```bash
    jupyter notebook notebooks/stock_price_model_prediction.ipynb
    ```

## Notebook Contents
- **Data Collection:** Merges stock price data from multiple CSV files for large-cap, mid-cap, and small-cap categories.
- **Data Preprocessing:** Prepares datasets by selecting relevant features such as Open, High, Low, Close, Adj Close, and Volume.
- **Model Selection and Training:** Utilizes Ridge Regression, RandomForestRegressor, and GradientBoostingRegressor. Implements a pipeline for data scaling and model fitting. Performs grid search with cross-validation to find the best hyperparameters for each model.
- **Evaluation and Results:** Splits the data into training and testing sets. Evaluates models based on mean squared error (MSE). Identifies Ridge Regression as the best model with the lowest MSE values for all stock categories.

## Results
- Large-Cap Stocks: Best Model - Ridge Regression, Training MSE - 515.29, Testing MSE - 1164.81
- Mid-Cap Stocks: Best Model - Ridge Regression, Training MSE - 2182.64, Testing MSE - 1321.33
- Small-Cap Stocks: Best Model - Ridge Regression, Training MSE - 1254.47, Testing MSE - 1101.69

## Contributing
Feel free to open issues or submit pull requests. Contributions are welcome!
