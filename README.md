# Neural Network Charity Analysis

# Overview
Beks, a data analyst, has been tasked with a final project to prove her data abilities. Primarily focusing on neural networks and machine learning. This project focuses on a foundation, called Alphabet Soup, that analysis businesses applying for funding and predicts which businesses to invest in.

## Data Source
The data source for this project is a CSV file with over 34,000 businesses who applied for funding with Alphabet Soup over the years. [Here](https://github.com/Sborresch/Neural_Network_Charity_Analysis/blob/main/charity_data.csv) is where the data source file can be accessed.

Here is a description of all the column names and meanings in the data source:
  - EIN and NAME—Identification columns
  - APPLICATION_TYPE—Alphabet Soup application type
  - AFFILIATION—Affiliated sector of industry
  - CLASSIFICATION—Government organization classification
  - USE_CASE—Use case for funding
  - ORGANIZATION—Organization type
  - STATUS—Active status
  - INCOME_AMT—Income classification
  - SPECIAL_CONSIDERATIONS—Special consideration for application
  - ASK_AMT—Funding amount requested
  - IS_SUCCESSFUL—Was the money used effectively

## Steps
1. Preprocess data for neural network model
2. Compile, train, and evaluate the model
3. Optimize the model
4. Create a report on findings for Alphabet Soup

# Results
## Data Preprocessing
### Target Variables
It is important to define what target variables are, also known as target outputs. These target variables can be singular or multiple in our machine learning model. These variables are depicted as "y" in standard TensorFlow documentation. Y or target variables are the dependent variables in our model.

![Screenshot](https://github.com/Sborresch/Neural_Network_Charity_Analysis/blob/main/Features_Targets.png)

For Beks Alphabet Soup neural network/machine model the target variables is the column name "IS_SUCCESSFUL". For our purposes, we want to build a model that will predict whether or not an applying business will be successful post investment. Therefore, we must separate the "IS_SUCCESSFUL" column from the rest of the input data. 

### Feature Variables
It is important to define what feature variables are, also known as input values. These feature variables can be singular or multiple in our machine learning model. These variables are depicted as "X" in standard TensorFlow documentation. X or feature variables are the independent variables in our model.

![Screenshot](https://github.com/Sborresch/Neural_Network_Charity_Analysis/blob/main/Features_Targets.png)

For Beks Alphabet Soup neural network/machine model the target variables is the column name "IS_SUCCESSFUL". For our purposes, we want to build a model that will predict whether or not an applying business will be successful post investment. Therefore, we must separate the "IS_SUCCESSFUL" column from the rest of the input data. However, the difference is that we will need to drop any "IS_SUCCESSFUL" columns with a "0" value. As, a "0" value means that the business was not successful post investment from Alphabet Soup. Therefore, we only want to use the data to teach out model for those successful businesses.

### Other Variables
There are 11 variables in the data source. Including EIN, NAME, APPLICATION_TYPE, AFFILICATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, IS_SUCCESSFUL. We have determined that the variable included in the target and features variable is IS_SUCCESSFUL. Therefore, the variables tha can be removed from the input data include, any "IS_SUCCESSFUL" variables with "0" value.

## Compiling, Training and Evaluating the Model
### Counts
![Screenshot](https://github.com/Sborresch/Neural_Network_Charity_Analysis/blob/main/Define_Model.png)

Looking at the model summary, we can see that the number of weight coefficients, also known as weight parameters, is calculated using this simple formula:
each layer = # of input values x # of neurons + bias term for each neuron.

Below is a count for each layer;
  - dense (Dense) = 44 ->(3520 param # / 80 neurons)
  - dense_1 (Dense) = 81 ->(2430 param # / 30 neurons)
  - dense_2 (Dense) = 31 ->(31 param # / 1 neurons)
  - total params = 5981
  - trainable params = 5981
  - non-trainable params = 0

### Model Performance

### Optimization

# Summary
## Results

## Recommendation

