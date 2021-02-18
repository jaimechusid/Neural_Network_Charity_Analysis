# Neural Network Charity Analysis

## Project Overview
The purpose of this analysis is to apply what we have learned about neural networks and machine learning to create a binary classifier that will predict whether or not applicants will be successful when funded by Alphabet Soup. To do so, I went through the steps of pre-processing data, compiling, training, and evaluating the neural networks model, and finally attempting to optimize the model to achieve a higher accuracy.

## Results

### Data Preprocessing
- The "Is Successful" variable was considered to be the target for my model.
- For the features of my model, I used the following variables: Application Type, Affiliation, Classification, Use Case, Organization, Income Amount, and Ask Amount.
- Ein and Name did not have to be included in the model because they are simply identifiers. Additionally, I chose not to use the Status and Special Considerations variables because they are both binary almost all rows had the same value. These four variables should be removed from the input data.

### Compiling, Training, and Evaluating the Model
- Initially, I used two hidden layers with 80 and 30 neurons, respectively. I used the RELU activation functions for the hidden layers and the sigmoid function for the output layer.
- After several attempts, I was not able to increase accuracy to achieve the 75% target model performance. I tried experimenting with several different changes, but was only able to increase accuracy ~1%.
- To try to increase model performance, I first dug deeper into the input values and determined the Status and Special Consideration variables were unneccessary to the analysis, so I removed them from the data. Then, I experimented with adding several more hidden layers, changing the number of neurons and epochs, and testing out different activation functions. However, I was still unable to make much of a difference to the accuracy.

## Summary
After optimization attempts, my model achieved around 54% accuracy and 69% loss. Because this is a binary classification model, I believe a Random Forest Classifier would be able to do a better job at accurately predicting the outcomes in this case. The dataset used in this project is tabular and can be preprocessed the same way to use in a Random Forest model. Because the accuracy did not change much as more epochs completed, I think it could benefit from the structure of a Random Forest model.
