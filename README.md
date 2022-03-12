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
<img width="755" alt="Capture2" src="https://user-images.githubusercontent.com/92502292/158036503-c1a207cb-4583-4012-9de2-788adedc8c5c.PNG">

- For the 3rd model (2nd optimiation) also has less and different input feature than the first optimization model. There are three hidden layer and more neurons numbers are added to each hidden layer. First and second layer has the activation of ReLU function and output has Sigmoid function in the model. This model yielded 0.7285 accuracy with 0.5690 loss value. Adding the additional layer in this model has slightly improved the model accuracy by a few points. 
<img width="844" alt="Capture3" src="https://user-images.githubusercontent.com/92502292/158036509-69cb3340-b4a4-4035-98f1-2dad5228558a.PNG">

- Most input features and hidden layer in 4th model (3rd optimization) are similar to model 3 but the activation function of each hidden layer has changed and only 50 epochs was applied to this model. For first layer and second layer, Tanh function was used and Linear function is used in the output layer. This model yielded 0.7279 accuracy and 0.6230 loss values. 
<img width="701" alt="capture4" src="https://user-images.githubusercontent.com/92502292/158036514-a7042fcb-8bc5-401d-8452-bd910b3625ae.PNG">


Recommdenation
Different machine leraning model such as RandomForest algorithm would be interesting to try with this datasets. It is because it has a few beneficial such as: 
- They are robust against overfitting as all the weak learners are trained on different pieces of data.
- It can be used to rank the importance of input variables in a natural way
- It run efficiently on large datasets. It can handle thousands of input variables without the deletion or dropping. 

