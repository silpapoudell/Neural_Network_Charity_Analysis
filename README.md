# Neural Networks and Deep Learning Models


## Overview of the analysis:

The purpose of the analysis is to implement the neural network or deep learning to predict which Alphabet Soup funded projects will use their funding successfully. 
Data Pre-processing, train and evaluate the model after that optimizing the model. 

## Results:

## Data Preprocessing

Variable that was considered as the target for my model: IS_SUCCESSFUL Column.

Variables that were considered features for my model: Every Column except for IS_SUCCESSFUL which is our target and the ones we will drop.

Variable that were neither targets or features for the dataset: Columns that I dropeed are EIN, NAME because they will have little to no impact om our outcome

The variable that should be removed are the identification variables: EIN and NAME. They are being excluded as they do not provide any additional data to the data set.


# Compiling, Training, and Evaluating the Model

For neural network model, we had 2 hidden layers.Our first layer had 80 neurons, the second has 30 there is also an output layer. The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."

Was the model able to achieve the target model performance?

The model was not able to reach the target 75%. The accuracy for my model was 69%.


## The steps taken to try and increase model performance

- Removed additional feature, that is the 'USE_CASE' column. Rest of the model components stayed the same, however model accuracy went down to 63%.

- Adding Additional neurons to hidden layers and additional hidden layers are added. The accuracy went down again, this time it was 53%.

- Changing activation function of output layer from "sigmoid" to "tanh." The accuracy of the model went down even more to 50%.



## Summary:

The Model got 50% accuracy after optimization. Initial neural Network had 69% accurary score. 
This loss in accuracy score can be explained from the facts that model got overfitted. 
We can increase the accuracy score by simply removing more features or adding more data to the dataset. 

Would like to recommend Random Forest Classifiers as it is robust and accurate model due to their sufficient number of estimators and tree depth.

Also the random forest models have a faster performance than neural networks and could have avoided the data from being overfitted.
