# Stock Prediction of Amazon 
Stock Prediction of Amazon using Recurrent Neural Network.
# Dataset
10 years of stock pricing data of Amazon is used for training and testing. The dataset is taken from yahoo finance's website in CSV format. 
# Data Pre-processing
The dataset is converted to OHLC average (Open, High, Low, Closing prices) and added as a new column. This has been converted into two column time series data, 1st column consisting stock price of time t, and second column of time t+1. All values have been normalized between 0 and 1.
# Model
Model has 4 layers. 2 layers of LSTM is used to buil the RNN model using keras library. Then dense layer is added. finally, "Liner" activation layer is added.
# Training
Adam optimizer is used for convergence. 
# Testing
Test accuracy metrics is mean absolute error.
# Perdiction
Next day's stock price and last day's stock price predicted by the model.
# Conclusion
OHLC average is used as other two parameters (HLC average and closing value) are not that significant. The training and testing error rate is 8.77 and 107.68 which training has low rate than testing. The model can be improved more by optimizing it.  
