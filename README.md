# Neural_Network_Charity_Analysis
## Overview of the analysis 
The purpose of this project is to use the machine learning and neural networks knowledge and apply on the features in the provided dataset. With the datasets, create a binary classifier that can help the foundation predict to make investments. 

## Results 
### Data Preprocessing 
- In this module, the "IS_SUCCESSFUL" is considered to be the target variable for this analysis. 
- The rest of the column become the input features after dropping IS_SUCCESSFUL column from the dataframe. 
- Non-beneficial ID columns, "EIN" and "NAME" which are neither targets nor features are removed from the input datasets in the data preprocessing step. 

### Compiling, Training, and Evaluating the Model 
- In the original analysis, 2 hidden layers with 80 neurons for first layer and 30 neurons for second hidden layer were used. Rectified Linear Unite (ReLU) function was used in both hidden layers. The output layer include only one neuron with linear Sigmoid function was selected. 
- The neural model with different parameters and features mentioned above was able to achieve the 72% of its accuracy. 
- To optimize the model performace over 75%, the steps such as removing non-beneficial feature was removed from the datasets, additional neurons to hidden layers and hidden layers were added to the model. The below screenshot is the accuracy and loss values of the first model after evaluation.
<img width="675" alt="capture" src="https://user-images.githubusercontent.com/92502292/158036491-a2536c67-3006-4ce5-ac49-f91de44b43ae.PNG">

## Summary 
- The first model with 2 hidden layers has the accuracy 0.7265 and loss of 0.5598. 
- The first optimation with second model has less input feature than the first model but the rest doesn't change. This model produced the accuracy of 0.7236 with 0.5882 loss value. 
- For the 3rd model (2nd optimiation) also has less and different input feature than the first optimization model. There are three hidden layer and more neurons numbers are added to each hidden layer. First and second layer has the activation of ReLU function and output has Sigmoid function in the model. This model yielded 0.7285 accuracy with 0.5690 loss value. Adding the additional layer in this model has slightly improved the model accuracy by a few points. 
- Most input features and hidden layer in 4th model (3rd optimization) are similar to model 3 but the activation function of each hidden layer has changed and only 50 epochs was applied to this model. For first layer and second layer, Tanh function was used and Linear function is used in the output layer. This model yielded 0.7279 accuracy and 0.6230 loss values. 

Overall, the 75% predictive accuracy wasn't achieved even with the three attemps optimization. The different machine learning such as RandomForest alogrithm should be considered to optimize the current datasets due to its robust against overfitting and am able to handle thousands of input variables without needing to deleting or dropping the datasets. The recommendation includes optimizing the number of neurons and acitivation function in each hidden layer.  



