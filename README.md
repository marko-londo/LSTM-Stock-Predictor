# Bitcoin Price Prediction with Deep Learning

This repository presents two distinct recurrent neural network models to predict Bitcoin's closing prices using LSTM (Long Short Term Memory) cells.

## Overview

1. **Closing Price Predictor**: This model employs a window of past closing prices to predict the `nth` closing price. For instance, if a window of 10 days is used, the model would take the closing prices of the previous 10 days to predict the 11th day's closing price.
2. **FNG Predictor**: This model utilizes the Fear and Greed (FNG) indicators to make its predictions about the closing price.

### Data Preparation

The dataset has been prepared, split, and normalized for training and testing. Appropriate data preprocessing steps ensure that the models receive the data in a format conducive to training.

### Model Construction and Training

Custom LSTM RNN models were built and trained to accommodate the specific nuances of Bitcoin's price movements.

### Evaluation

Both models underwent thorough evaluation to compare their performance:

- **Closing Price Predictor**: Achieved a loss of `0.013043398037552834`.
- **FNG Predictor**: Noted a loss of `0.13850949704647064`.

Clearly, the Closing Price Predictor outperformed the FNG Predictor in terms of accuracy.

### Visualization

Visual comparisons between actual vs. predicted values were drawn for both models:

- The **Closing Price Predictor** showcased an impressive performance, with its predictions closely mirroring the actual data.
- The **FNG Predictor**, on the other hand, managed to capture the overall trend decently but fell short of pinpointing the exact values.

#### Best Time Window

The most effective time window for making predictions was found to be 1 day. This makes intuitive sense since cryptocurrency markets, especially Bitcoin, are highly volatile and are influenced by a multitude of factors on a day-to-day basis. Using a short window ensures that the model is trained on the most recent and relevant data.

### Visualizations

To view the visualizations of each model's performance, use the following code:

```python
# Replace this placeholder with your code to display images of each visualization.
