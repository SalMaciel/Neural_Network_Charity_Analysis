# Neural_Network_Charity_Analysis
## Overview
In this project we will be looking at a dataset containing over 34,000 organzations that received funding from Alphabet Soup. The objective is to create a neural network that help predict if a specific project is likely to fail or succeed, and thus, make better decisions when funding said projects.
## Results
Data preprocessing. At first glance columns EIN and NAME pop out immediatly as not needed. Out target is the column IS_SUCCESSFUL.

![data frame preview](images/first.PNG)  
![dropping unwanted columns](images/first_drop.PNG)  
![identifying target column](images/target.PNG)  

For our first model, the input layer has the same amount of nodes as features, 2 hidden layers with 40 and 20 nodes and relu as the activation function, the output layer has sigmoid as activation function.
![defining first model](images/first_model_layers.PNG)  
![first model results](images/first_model.PNG)  
![defining second model](images/sec_model_layers.PNG)  
![second model results](images/sec_model.PNG)  
![defining last model](images/fourth_model_layers.PNG)  
![last model results](images/fourth_model.PNG)  