# Crypto study

This document is a study for investigate an propose some trading simulations using different types of data science techniques.

## How to proceed with this document

The idea is to get conclusions of the tests to perform.

## Proposed strategies

- Neural networks for predicting global graphics
- Neural networks for predicting quick changes in multiple markets
- Linear function GRID

## Neural networks for predicting global graphics

Solutions based on neural networks.

### LSTM layers

It evaluates only the following register.

Proposal:

- Use the predicted value as training value for multiple day predicting.

## Neural networks for predicting quick changes in multiple markets

This strategy tries to predict in a market if there's going to be a rise of a specific percentage of the price. Returning a value closer to 1 or 0.

Data training: {"List_of_prices": [], "Expected_output": boolean}

- Supervised contrastive learning
  - https://keras.io/examples/vision/supervised-contrastive-learning/
- LSTM layers (Long Short Term Memory)
  - https://machinelearningmastery.com/time-series-prediction-lstm-recurrent-neural-networks-python-keras/
  - https://towardsdatascience.com/machine-learning-recurrent-neural-networks-and-long-short-term-memory-lstm-python-keras-example-86001ceaaebc
  - https://wandb.ai/ayush-thakur/dl-question-bank/reports/LSTM-RNN-in-Keras-Examples-of-One-to-Many-Many-to-One-Many-to-Many---VmlldzoyMDIzOTM
  - https://www.tensorflow.org/guide/keras/rnn
  - https://machinelearningknowledge.ai/keras-lstm-layer-explained-for-beginners-with-example/
- Supervised learning
  - .
- Classification techniques (classify on keep-stable, rise, fall)
  - https://www.tensorflow.org/tutorials/keras/classification?hl=es-419
  - https://www.pluralsight.com/guides/classification-keras
  - https://machinelearningmastery.com/sequence-classification-lstm-recurrent-neural-networks-python-keras/ Sequence classification
  - https://www.tensorflow.org/text/tutorials/text_classification_rnn
  - https://www.analyticsvidhya.com/blog/2021/06/lstm-for-text-classification/

## Linear function GRID

- To get a math model in order to get "floor" and "ceil" prices
- Obtain a number between 0 and 1 depending of the current price in reference to the floor and the ceil
- To select a collection of cryptocurrencies for the balance
- To find a way to balance a quantity between the markets... To buy all to the max profitability? -> First prototype
- To develop the algorithm for MTR-ENGINE

## Conclusions

### LSTM Full graphic evaluation

A price can be estimated based on the previous prices.

Test 1: Predict day to day based on the previous 30 days.
