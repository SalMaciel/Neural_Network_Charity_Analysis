# Neural_Network_Charity_Analysis
## Overview
In this project we will be looking at a dataset containing over 34,000 organzations that received funding from Alphabet Soup. The objective is to create a neural network that help predict if a specific project is likely to fail or succeed, and thus, make better decisions when funding said projects.
## Results

- What variable(s) are considered the target(s) for your model?
    - "IS_SUCCESSFULL" column.
- What variable(s) are considered to be the features for your model?
    - Every other column is used as features.
- What variable(s) are neither targets nor features, and should be removed from the input data?
    - "EIN" and "NAME" coumns.
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - For the first model we used one hidden layer with 40 nodes and one with 20 nodes and both with activation function relu. All these was chosen at random just to get started.
- Were you able to achieve the target model performance?
    - No.
- What steps did you take to try and increase model performance?
    - Lower the number of features and added more hidden layers and nodes.  

Data preprocessing. At first glance, columns 'EIN' and 'NAME' pop out immediatly as not needed. Our target is the column 'IS_SUCCESSFUL'. Every other column will be used as features.
![data frame preview](images/first.PNG)  
![dropping unwanted columns](images/first_drop.PNG)  
![identifying target column](images/target.PNG)  

For our first model, the input layer has the same amount of nodes as features, 2 hidden layers with 40 and 20 nodes and relu as the activation function, the output layer has sigmoid as activation function.
![defining first model](images/first_model_layers.PNG)  
![first model results](images/first_model.PNG)  

For the second model, the only difference is that we doubled the number of nodes in the hidden layers, everything else stayed the same way. This model showd no improvement over the first one.
![defining second model](images/sec_model_layers.PNG)  
![second model results](images/sec_model.PNG)  

For the last model, we lower the ammount of columns by combining them in the "other" categorie and by removing the column 'SPECIAL_CONSIDERATIONs_N' and added a third hidden layer, every layer has different activation function. This model showd no improvement over the previous ones.
![defining last model](images/fourth_model_layers.PNG)  
![last model results](images/fourth_model.PNG)  
## Summary
None of the models created performed at 75% or better. The number of layers nodes and activation functions used were chosen completly at random; however, both training and training sessions seemed to plateau fairly quickly, and adding layers and nodes did not made the model perform better, if any, slighlty worse. To create a better model I recomend spending more time understanding the data and keep trying different models with different activation functions such us "tanh" and "sigmoid" in the hidden layers.