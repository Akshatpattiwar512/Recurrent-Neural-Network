# Recurrent-Neural-Network

A recurrent neural network (RNN) is a type of artificial neural network in which node connections form a directed graph along a time sequence. As a result, it can display temporal dynamic behaviour. RNNs, which are derived from feedforward neural networks, can handle variable length sequences of inputs using their internal state (memory). As a result, they may be used for tasks like unsegmented, linked handwriting recognition or speech recognition. Recurrent neural networks are Turing complete in theory and may execute arbitrary algorithms to handle arbitrary sequences of inputs.

Implementation of RNN
1.Importing libraries
2.Splitting dataset
3.Data processing
4.Model Building
5.Prediction
6.Visualization


## BTC_Price_Prediction_Using_RNN
The bitcoin system consists of a collection of decentralised nodes that execute the bitcoin code and store the blockchain. No one can trick the system since all computers running the blockchain have the same list of blocks and transactions and can watch these fresh blocks being filled with new bitcoin transactions in real time.
Using RNN- Future bitcoin prediction is made from the available data

Dataset taken from kaggle: https://www.kaggle.com/mczielinski/bitcoin-historical-data


## Energy_Consumption_Prediction_using_RNN_and_LTSM

### LSTM
RNNs can recall inputs for a long time because of LSTMs. This is due to the fact that LSTMs store information in a memory, similar to a computer's memory. The LSTM has the ability to read, write, and erase data from its memory.An LSTM has three gates: input, forget, and output. These gates decide whether to allow fresh input (input gate), discard the information because it isn't relevant (forget gate), or let it affect the output at the current timestep (output gate).
Trend of energy consumption is used for predicting 
Hourly data is used 
Dataset taken from kaggle: https://www.kaggle.com/robikscube/hourly-energy-consumption


## Google_stock_price_prediction_RNN
Predicting stocks of google on the basis of previous stock data available
Dataset link: https://www.kaggle.com/ptheru/googledta


## Reber_Grammar_Classification
In this project, I constructed an RNN to classify whether or not a string matched the embedded Reber Grammar


### ERG-conforming strings
Ultimately, the data that I feed into this keras-based RNN had to be a matrix numerically representing strings. Each value in the matrix represented the index of a particular character in the reber alphabet BEPSTVX, or it contained a padding character. First, I had to synthetically generate examples of strings that matched the ERG and strings that did not. Sampling from the ERGs was pretty simple: I constructed the grammar as a graph, and as I traversed the graph, whenever I came upon a node with multiple outgoing edges, I simply chose one uniformly randomly until I reached the final node. I discarded any strings that exceeded a max_length (since they all had to fit into a rectangular matrix).
### non-ERG-conforming strings
However, coming up with the strings that didn't match the ERG required an iterative process.


## Time_Series_Forecasting_Using_Recurrent_Neural_Networks(RNN)
Time series forecasting is the process of making scientific forecasts based on time stamped data from the past. It entails developing models based on previous data and utilising them to make observations and drive future strategic decisions.
Time series prediction problems are a difficult type of predictive modeling problem.
Unlike regression predictive modeling, time series also adds the complexity of a sequence dependence among the input variables.
A powerful type of neural network designed to handle sequence dependence is called recurrent neural networks. The Long Short-Term Memory network or LSTM network is a type of recurrent neural network used in deep learning because very large architectures can be successfully trained.
LSTM networks in Python using the Keras deep learning library is developed to address a demonstration time-series prediction problem.

zip file used: https://storage.googleapis.com/tensorflow/tf-keras-datasets/jena_climate_2009_2016.csv.zip 

## For google colab users
Dataset can be directly imported without downloading. Follow the steps below:
! pip install kaggle
! mkdir ~/.kaggle
! cp kaggle.json ~/.kaggle/
! chmod 600 ~/.kaggle/kaggle.json
! kaggle datasets download <data name>  #Eg: for google stock prediction use ! kaggle datasets download mczielinski/bitcoin-historical-data
! unzip <Enter_zip_filename_from_the_output_of_the_above_code>  #Eg: ! unzip googledta.zip
