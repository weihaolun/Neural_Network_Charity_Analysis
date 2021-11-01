# Neural Network Charity Analysis with Neural Networks and Deep Learning

## Overview

### Background

Beks is a data scientist and programmer for the nonprofit foundation, Alphabet Soup. Now, she is going to put her skills to work to help the foundation predict where to make investment. From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.

### Purpose

I will use my knowledge of machine learning and neural networks and use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applications will be successful if funded by Alphabet Soup.

There are four deliverables in this project:

1.	 Preprocessing Data for a Neural Network Model
2.	 Compile, Train, and Evaluate the Model
3.	 Optimize the Model
4.	 A Written Report on the Neural Network Model 

## Results

### Data Preprocessing

- **What variable(s) are considered the target(s) for your model?**

    The target is the binary feature “IS_SUCCESSFUL”, which indicates whether the money was used effectively. 

- **What variable(s) are considered to be the features for your model?**

    "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT", "STATUS", these columns are features for the model.

- **What variable(s) are neither targets nor features, and should be removed from the input data?**

    “EIN” and “NAME” are identification columns, have been removed from the input data.

### Compiling, Training, and Evaluating the Model

- **How many neurons, layers, and activation functions did you select for your neural network model, and why?**

     The neural network model has 2 hidden layers with 80 and 30 neurons for each layer. Generally, it is common to choose 2 layers, 80 is close to twice of input features (43) and 30 is close to 2/3 of the input features. I used ```ReLU``` activation function to for hidden layers to speed up the training process and used ```Sigmoid``` for the binary output layer.


- **Were you able to achieve the target model performance?**

     The performance is around 73%, which is below target model performance of 75%.

- **What steps did you take to try and increase model performance?**
    1.	Applied bucketing to ASK_AMT feature.
    2.	Added additional neurons on hidden layers.
    3.	Added additional hidden layers.
    4.	Used different activation function, tanh.


