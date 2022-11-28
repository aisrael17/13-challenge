# 13-challenge

## Data
For this challenge, I used a dataset of organizations that have received funding from Alphabet Soup, a venture capital firm, over the years. This CSV contained a variety of information about the businesses, which I used to predict whether the businesses would ultimately become successful.

## Technologies
For this challenge, I used the following libraries in Python 3:
* pandas
* tensorflow (Dense, Sequential)
* sklearn (train_test_split, StandardScaler, OneHotEncoder)
* Google Colab

## Process & Results
First, I loaded in the data and used OneHotEncoder to transform the categorical variables into numerical data. Then, I split the data into a training and test set and used StandardScaler to transform the feature set. Last, I designed, trained, and tested a neural network to predict the success of the various businesses in the dataset. My first model was structued with:
* An input layer consisting of 116 nodes 
* 2 hidden layers
  * One with 55 nodes nodes (relu activation)
  * One with 25 hidden nodes (relu activation)
* An output layer (sigmoid activation), predicting whether or not a business will be successful

The model did not improve with more epochs of training and tapped out around a loss of 0.56 and accuracy of 73.0%. I then tried two different architectures, one with a single hidden layer of 75 and one with a single hidden layer of 25. Despite the changes, the accuracy did not improve. The 75-node model had loss of 0.57 and accuracy of 72.8% and the 25-node model had 0.56 loss and 72.7% accuracy. 

