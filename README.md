# Parallel_Stocks

This project aims to predict the stocks in the future using support vector machines and comparing with an RNN in serial and parallel computing. It aims to disagree with the Effective Market Hypothesis(EMH) which states that you cannot predict a stock in the future.

It also aims to check the time complexity of not only between algorithms but also comparing the same algorithm between serial and parallel computing to see if parallel computing is worth in such a situation.

## SVR

A Support Vector regressor was trained with a window prediction size of 30 days. The data taken as x variable was the close column of the stock dataset and the y variable was the close prices after 30 days. The kernel used was a rbf kernel with gamma value as 0.01. The model turns to perform decently with an accuracy of approximately 55%. 

## RNN (LSTM)

A reccurent neural network stands out of others as it can retain and use previous data for future predictions. A problem with rnn is that they can only retain only short period of information. A solution to this is the LSTM(Long Short term model) which can retain long periods of information. 
An LSTM model was trained using tensorflow2.0 beta. The results turn out to be pretty convincing with an mean absolute error of about 20.
