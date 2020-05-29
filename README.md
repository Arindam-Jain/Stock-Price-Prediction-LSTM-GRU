# Stock-Price-Prediction-LSTM-GRU

# DATA USED:
  GOOGL stock daily closing price from 19.08.2004 to 28.03.2019 (working days- 3677 rows)

● Data is split into training and testing data in the ratio 80:20.
● Each of traning and testing data is transformed from a vector containging
closing prices to a dataset with ‘look_back’ number of preceding stock prices as independent variables (features) and future stock price as the independent variable.
● The data is standardized before being used for training.

# Architechture of LSTM network:
Input dimension: (1, look_back)
Layer 1: LSTM with output dimension - 50
Dropout of 0.5 is added
Layer 2: LSTM with output dimension - 100
Dropout of 0.2 is added
Layer 3: Dense with output dimension - 1 (Output of the network) Network is trained for 800 epochs with batch_size 20.

# Architechture of GRU network:
Input dimension: (1, look_back)
Layer 1: GRU with output dimension - 50
Dropout of 0.5 is added
Layer 2: GRU with output dimension - 100
Dropout of 0.2 is added
Layer 3: Dense with output dimension - 1 (Output of the network) Network is trained for 800 epochs with batch_size 20.

