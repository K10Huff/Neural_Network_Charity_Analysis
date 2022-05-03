# Neural Network Charity Analysis

# Overview of the Analysis
The purpose of this analysis was to employ deep learning neural networks in order to predict a successful contribution to a charitable organization in order to assist with future predictions and investments.. The goal was to build a binary classifier based off previous charitable donations and metrics describing the organizations that were funded.

# Results
-	Data Preprocessing
    - The target for this model was the column: IS_SUCCESSFUL
    - The features of this model were the columns: APPLICATION_TYPE, AFFILIATION CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
    - The variables removed from the dataset as they were not the target nor were they features were the non-beneficial ID columns, 'EIN' and 'NAME'
-   Compiling, Training, and Evaluating the Model
    - The final model that yielded the best results had 3 hidden layers, with 500, 300, and 25 perceptrons within the layers. The activation functions were ReLU and sigmoid. The output function was sigmoid as that is the best output function for giving a classification probability. The adam optimizer was used to overcome week features in the dataset and the loss function chosen was the binary_crossentropy because it is the most suited for binary classification models. 
    - The target model performance of 0.75 was not achieved, the model was only able to yield 0.7239 accuracy.
    - In order to try and increase model performance the number of hidden layers, the number of perceptron in each layer, the activation functions, output functions and additional dropped columns (STATUS) were all tested to find the combination that yielded the best results.
# Summary: 
### Results Table <br>
![Advanced Confusion Metrics DF](https://github.com/K10Huff/Neural_Network_Charity_Analysis/blob/3cc3e07764642b5019037cf059867fefdc590339/resources/acm_df_new.png) <br>
The final model was not able to yield an accuracy of 0.75. Instead of using a binary classification model with a successful/ not successful target, an alternative would be to use a mulit-classifcation model. The target column could instead hold an evaluation score with values like “not successful, moderately successful, successful” to allow the model a third value to more accurately define the clusters of organizations. 
