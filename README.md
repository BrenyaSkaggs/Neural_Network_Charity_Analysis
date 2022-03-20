
## Overview 

Assist Alphabet Soup with data containing 34,000 organizations that have received funding over the years. With this data we will create a binary classifier in predicting whether 
applicants will be successful wiht funding by Alphabet Soup.




## Results 

### Data Preprocessing

* What variable(s) are considered the target(s) for your model?
Our target is IS_SUCCESSUL. This is also the output for the organizations that received funding over the years.


* What variable(s) are considered to be the features for your model?
The following variables are considered to be features: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CAE, ORGANIZATION,
STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT ADN IS_SUCCESSFUL.


* What variable(s) are neither targets nor features, and should be removed from the input data?
We removed EIN and NAME from the data.


### Compiling, Training, and Evaluating the Model'

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
The original neural network model consisted of two layers, 30 neurons in the first layer and 15 in the second. The ReLU activation function was used to enable nonlinear
relationships. While trying to reach the accuracy goal of 75% I increased neurons, added an additional layer and changed the function from ReLU to Tanh. The closest 
I was able to get was 72% accuracy.



* Were you able to achieve the target model performance?
No, none of the models were able to achieve the 75% target. 



* What steps did you take to try and increase model performance?

1. Removed two additional columns to reduce noise. Columns removed were EIN, NAME, ORGANIZATION and SPECIAL_CONSIDERATIONS.
![This is an image](https://raw.githubusercontent.com/BrenyaSkaggs/Neural_Network_Charity_Analysis/main/Resources/Removing%20additional%20columns.png)

2. Added additional neurons to the two exisitng hidden layers. 
![This is an image](https://raw.githubusercontent.com/BrenyaSkaggs/Neural_Network_Charity_Analysis/main/Resources/Additional%20Neurons.png) 

3. Added an additional hidden layer. 
![This is an image](https://github.com/BrenyaSkaggs/Neural_Network_Charity_Analysis/blob/main/Resources/Third%20hidden%20layer.png)

4. Changed the activation feature to tanh.
![This is an image](https://raw.githubusercontent.com/BrenyaSkaggs/Neural_Network_Charity_Analysis/main/Resources/Change%20Feature.png)



## Sumary 

The deep learning neural network model was unable to meet the 75% accuracy target. I would recommend using Random Forest Classifier to help prevent overfitting.

