# Neural_Network_Charity_Analysis
## Overview

   From Alphabet Soup’s business team, I received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

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
- IS_SUCCESSFUL— Was the money used effectively
Develop neural network to predict if the funding was used effectively or not. 
## Result
### Data Processing
1. Variable that considered the target for my model : IS_SUCCESSFUL
2. Features hat considered the target for my model : APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT. 
3. Removed inputs from the data : EIN and NAME, the identification columns are not useful for the prediction. 
### Compiling, Training, Evaluating the Model
![](https://user-images.githubusercontent.com/64121596/159072793-23bc8819-f047-4783-ace1-d2633b6eccfe.png)
4. From the above picture, I chose 2 hidden layers with "Relu" activation function, and for the output  layer, I chose sigmoid acti ation function. 
5. The performance was : Loss: 0.5565535426139832, Accuracy: 0.7259474992752075. I didn't achieve the target accuracy of 75%. 
6. (Picture below)I tried binning less in the  classification column, tried Random Forest and SVM. Which also gave me accuracy less than 75%. I tried adding another layer and changing the activation function from relu to tanh. When the activation function is tanh, it gave worse result, so I changed it back to relu. Changing the epochs to 100 didn't affect the accuracy as well.  The model accuracy was still under 75%. 
![](https://user-images.githubusercontent.com/64121596/159074643-47494b6c-5f5f-4546-bfd9-5d934544d478.png)
## Summary
The neural network was not working well in this dataset. We need to dig deeper in changing the activation function and adding layers. In this particular dataset, we should try different machine learning algorithm.
