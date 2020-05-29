# Stock-Price-Prediction-LSTM-GRU

# DATA USED:
  GOOGL stock daily closing price from 19.08.2004 to 28.03.2019 (working days- 3677 rows) </br>

● Data is split into training and testing data in the ratio 80:20.</br>
● Each of traning and testing data is transformed from a vector containging</br>
closing prices to a dataset with ‘look_back’ number of preceding stock prices as independent variables (features) and future stock price as the independent variable.</br>
● The data is standardized before being used for training.</br>

# Architechture of LSTM network:
Input dimension: (1, look_back)</br>
Layer 1: LSTM with output dimension - 50</br>
Dropout of 0.5 is added</br>
Layer 2: LSTM with output dimension - 100</br>
Dropout of 0.2 is added</br>
Layer 3: Dense with output dimension - 1 (Output of the network) Network is trained for 800 epochs with batch_size 20.</br>

# Architechture of GRU network:
Input dimension: (1, look_back)</br>
Layer 1: GRU with output dimension - 50</br>
Dropout of 0.5 is added</br>
Layer 2: GRU with output dimension - 100</br>
Dropout of 0.2 is added</br>
Layer 3: Dense with output dimension - 1 (Output of the network) Network is trained for 800 epochs with batch_size 20.</br>

