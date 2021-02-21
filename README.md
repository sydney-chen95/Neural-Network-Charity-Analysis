# Neural-Network-Charity-Analysis

## Purpose
The purpose of this project is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup Charity Group with the knowledge of machine learning and neural networks.


## Results

#### Data Preprocessing
 
- What variable(s) are considered the target(s) for your model?
    
    The target variable for this model is IS_SUCCESSFUL.

- What variable(s) are considered to be the features for your model?

    The features variables for this model are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT.

- What variable(s) are neither targets nor features, and should be removed from the input data?

    The variables removed from this model are EIN and NAME.

#### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

    For this model, the number of layers and neurons were chosen from the guidelines of a basic neural network where it is recommended to have 2-3 times the amount of neurons in the hidden layers as the input amount. The activation functions I chose were relu and sigmoid. 

- Were you able to achieve the target model performance?

 ![Initial Model accuracy](https://github.com/sydney-chen95/Neural-Network-Charity-Analysis/blob/main/Images/Initial%20Model%20accuracy.png?raw=true)
    
   I was unable to achieve the target model performance. My model's accuracy was only 72.56%.

- What steps did you take to try and increase model performance?

 ![Optimized Model accuracy](https://github.com/sydney-chen95/Neural-Network-Charity-Analysis/blob/main/Images/Optimized%20Model%20accuracy.png?raw=true)

   My attempt at optimizing the model's performance was to remove AFFILIATION column from the dataset, increased the number of values for each bin, and adding additional hidden layer to the model. However, this did not increase mdoel performance at all. Instead, this new model's accuracy decreased to 65.55%.

## Summary: 

   The goal of this project was to create a model to predict the successfulness of candidates who will receive a donation from Alphabet Soup Charity. We used deep learning neural network models to estimate the ability of the models created, trained and defined using a dataset of known successful companies that have received donations. The models were aimed to have at least a 75% accuracy and inorder to increase its performance, the model parameters were modified by removing noisy variables, changing bin values and increasing hidden layers. However, this did not increase the model's performance and instead dropped from an accuracy score of 72.56% to 65.55%. 
    
   My recommendation for a different model would be Random Forest Classifiers. This ensemble learning method for classification will construct multiple decision trees to predict accuracy and control over-fitting. 
