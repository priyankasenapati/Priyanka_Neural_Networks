# Priyanka_Neural_Networks:- 

# Overview:-

Neural Networka and Deep Learning Models, In this module, I have build a machine learning model to predict the success of charity ventures paid by Alphabet soup using TensorFlow library and Keras module. The Alphabet Soup Charity dataset is provided in a csv file contains funding information for 34,300 charity ventures. I will be using this to train and test the models.

# Data and Resources:-
 * Software: Python 3.7.6, Pandas, Scikit-learn, Tensor Flow
 
 * Dataset: charity_data.csv

### Summary of Results:

1- The target variable would be IS_SUCCESSFUL since we are trying to find if funding a startup will be successful or not. 

2- The variables that are considered to be the features are: ASK_AMT, USE CASE, ORGANIZATION, INCOME_AMT.

3- Other variables were processed as follows:
* NAME - Non feature or target.

* STATUS - Non feature or target.

* CLASSIFICATION - Check unique value counts to decide if binning is recommended. Was binned.

* APPLICATION_TYPE - Was binned.

* SPECIAL_CONSIDERATIONS_Y was dropped since it is binary valued.

4- Rare categorical values were combined using bucketing: Bucketed APPLICATION_TYPE and CLASSIFICATION. I fit the OneHotEncoder() and produced the encoded DataFrame. Numeric value were standardized using Tensor flow’s StandardScalar Class.

5- I created the Tensor flow Keras Sequential Classifier using tf.keras.models.Sequential(). Also I used 2 hidden layers with 200  neurons in the first and 55 in the second. Then I used 3 hidden layers with 100, 100 and 50 neurons in each layer respectively.

6-To increase the model accuracy, I did the following:

* Increased the number of hidden layers to 3, Increased the number of neurons per layer to 100, 100 and 55.

7-I was able to achieve the target predictive accuracy of 75%

8- Since Alphabet Soup required an outcome of IS_SUCCESSFUL or NOT, which is binary, I would have used a Random Forest Classifier. It would also take less time train.
