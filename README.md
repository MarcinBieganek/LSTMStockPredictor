# Stock Price Prediction with LSTM for Dino S.A.

## Project Overview

This project aims to forecast the future stock prices of Dino S.A., a Polish retail company, using a Long Short-Term Memory (LSTM) neural network. The model is trained on historical daily stock data from **April 2017 to April 2025** to predict future closing prices.

The primary goal is to build and evaluate an effective time-series forecasting model using machine learning techniques.

## Dataset

The dataset was sourced from the Polish financial portal **stooq.pl** and includes daily stock quotations (Open, High, Low, Close) for Dino S.A.

## Methodology

1.  **Data Preprocessing**: The historical data was loaded, and two different scaling techniques were tested for their impact on model performance: `MinMaxScaler` and `StandardScaler`.
2.  **Model Architecture**: An LSTM-based neural network was designed and implemented using TensorFlow and Keras.
3.  **Training & Evaluation**: The model was trained on a subset of the historical data and then evaluated on a separate test set. Its predictions were plotted against the actual closing prices to visually assess performance.

## Key Findings & Conclusion

- The LSTM model's performance was highly dependent on the data scaling method. The model using **`MinMaxScaler`** provided more accurate and stable predictions.
- The model with **`StandardScaler`** tended to overfit the training data, resulting in poorer generalization on the test set.
- The project confirms that while LSTMs are a powerful tool for time-series forecasting, success is heavily reliant on proper data preparation and a well-configured model architecture.

## Potential Improvements

- Enrich the dataset with additional features, such as trading volume, technical indicators, or broader market indices.
- Experiment with deeper or different recurrent architectures (e.g., GRU layers, stacked LSTMs).
- Conduct more rigorous model validation across different market conditions and time periods.