# **Neural_Network_Charity_Analysis**


## **Overview** 

The purpose of the analysis is to utilize machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
In this module we used the Keras module to build the neural network.

## **Results**


1) **What variable(s) are considered the target(s) for your model?**
APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

2) **What variable(s) are considered to be the features for your model?**
The dependent feature of the model = ['Is_Successful']

3) **What variable(s) are neither targets nor features, and should be removed from the input data?**
These objects were removed from the data: columns=['EIN','NAME']


**Compiling, Training, and Evaluating the Model**

**How many neurons, layers, and activation functions did you select for your neural network model, and why?**
1) The original model requested 2 hidden layers with relu activation inputs, and sigmoid output. 
 
**Were you able to achieve the target model performance of 75%?**
2) No. I did try multiple items and received about a 66% as highest. 

**What steps did you take to try and increase model performance?**
1) Removed additional variables that may have had noise or were duplicates in general behavior: Status, Income_Amt, Ask_Amt. 

### ![Pass1](https://github.com/ljlodl5/Neural_Network_Charity_Analysis/blob/main/removedcolumns66.PNG)

2) Added a hidden layer and increased nodes with a 3rd layer. 

### ![Pass2](https://github.com/ljlodl5/Neural_Network_Charity_Analysis/blob/main/addedhiddenlayer53.PNG)

3) Changes activation from relu to tanh. 

### ![Pass3](https://github.com/ljlodl5/Neural_Network_Charity_Analysis/blob/main/changedtotanh37.PNG)

## Summary
There are other items I could have considered: increasing epochs, organizing values into 'Other' categories, adding data, changing the model. 
Other supervised models with less columns may actually perform better. Sometimes simplifying the existing categories can perform better as well. I feel this particular dataset and model was successful only to a point, there were too many variables and when compounded by the hidden layers 
the inability to detect binary division was evident.




