# Bitcoin Price Prediction with Deep Learning

In this repository, I leverage recurrent neural networks using LSTM (Long Short Term Memory) cells to predict Bitcoin's closing prices. The exact same model architecture and random seed have been employed across two distinct notebooks, ensuring consistency in the modeling approach.

## Overview

1. **Notebook 1 - Closing Price Predictor**: This notebook focuses on using a window of past closing prices to predict the `nth` closing price.
2. **Notebook 2 - FNG Predictor**: The emphasis of this notebook is on employing the Fear and Greed (FNG) indicators as features to predict the closing price.

### Data Preparation

Both notebooks follow an identical process where the dataset is prepared, split, and normalized for training and testing. Such preprocessing ensures a consistent input format for our LSTM RNN model.

### Model Construction and Training

The same custom LSTM RNN model was replicated across both notebooks for training on different sets of features.

### Evaluation

A comparison of performance between the two models revealed:

- **Closing Price Predictor**: Achieved a loss of `0.013043398037552834`.
- **FNG Predictor**: Posted a loss of `0.13850949704647064`.

Despite the similarity in architecture, the Closing Price Predictor evidently delivered superior results compared to the FNG Predictor.

### Visualization

Visual comparisons between actual vs. predicted values were created:

- The **Closing Price Predictor** exhibited exceptional alignment with the actual data, closely tracing its fluctuations.
- The **FNG Predictor** managed to emulate the broader trend but didn't always precise values.

#### Best Time Window

The 1-day window emerged as the most effective for making predictions. Given Bitcoin's notorious volatility and the plethora of daily influences, a short window allows the model to train on the freshest, most pertinent data.

### Visualizations
#### Closing Price Predictor
![Closing Price
Predictor](https://github.com/marko-londo/LSTM-Stock-Predictor/blob/main/Visualizations/closing.png?raw=true)
#### FNG Predictor
![FNG Predictor](https://github.com/marko-londo/LSTM-Stock-Predictor/blob/main/Visualizations/closing.png?raw=true)