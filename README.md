# Fish
Using a dataset of various fish species, we aim to predict the weight of the Bream species fish based on certain characteristics such as vertical length, diagonal length, cross length, height, and width. We'll employ the Linear Regression method to determine the relationship between these characteristics and the fish's weight.

Species: The species name of the fish

Weight: The weight of the fish in grams

Length1: Vertical length in centimeters

Length2: Diagonal length in centimeters

Length3: Cross length in centimeters

Height: Height in centimeters

Width: Diagonal width in centimeters

## Data Exploration
Fish data set was explored by looking at the first few records and summary statistics of each column and renamed the column to get easy understanding of each variables name.
![image](https://github.com/user-attachments/assets/855cd03e-42d0-4750-8c03-b6c0a0872208)
![image](https://github.com/user-attachments/assets/95ab1724-e16c-46d9-9837-cd9c1be2690f)
![image](https://github.com/user-attachments/assets/a27e4467-0afa-42c2-a93c-47502733af2d)
Then identified correlation between numerical variables of fish dataset. 
![image](https://github.com/user-attachments/assets/50bae631-e35a-46a5-b8ab-13b91e6d12ca)

## Data Exploration
![image](https://github.com/user-attachments/assets/8cd4ee48-4a64-4c6d-bc22-693e1dcdca05)
The diagram above visually represents the relationship between fish weight and vertical length, demonstrating a clear trend where fish weight increases with greater vertical length. The diagram below depicts the distribution of fish weights and vertical lengths across different species, highlighting variations in these characteristics among the species.
![image](https://github.com/user-attachments/assets/27393aa1-f1c6-47ec-a80e-03b6a2b52d4f)
Below graph illustrates the distribution of Bream species fish weights, providing insights into how weight varies at different length.
![image](https://github.com/user-attachments/assets/c5bdb16a-3d5d-4e57-9925-e9069a0193a8)

## Model Building - Linear Regression
To predict the weight of Bream species fish using a linear regression model, we follow these steps:
Data Preparation:
Ensure that there are no missing or inconsistent values in the dataset, especially in the target variable (weight) and the predictor variables (vertical length).
Data Partitioning:
Splitting the Dataset: The entire dataset is divided into two subsets: a training set and a testing set. The training set is used to build and train the model, while the testing set is used to evaluate the model's performance. A common split ratio is 80% for training and 20% for testing.
For the Bream species, vertical lengthis used as predictor variables.
A linear regression model is applied to the training data to establish a relationship between the fish's weight and its vertical length. The model aims to find the best-fitting linear equation.

The trained model is applied to the testing dataset to predict the weight of Bream species fish. The predicted weights are then compared to the actual weights in the test set. To evaluate the accuracy of the model, various metrics can be used, such as Mean Absolute Error (MAE), and R-squared (R²). These metrics help in understanding how well the model predicts the target variable.
Analyzing the coefficients (β values) provides insights into how each characteristic influences the weight of the Bream species fish. For instance, a higher coefficient for vertical length would indicate a stronger positive relationship between vertical length and weight. The R-squared value indicates the proportion of the variance in the dependent variable (weight) that is predictable from the independent variables (fish characteristics). A higher R-squared value suggests a better fit of the model to the data. This process enables us to predict the weight of Bream species fish based on their physical characteristics with a quantified measure of confidence in the predictions.
![image](https://github.com/user-attachments/assets/c710028d-6f2b-4bb0-934a-7ca7ca682f95)
![image](https://github.com/user-attachments/assets/9ef1cb12-d80f-4673-b3d6-6176e59a732a)
The diagram shows how far predicted value is falling from the actual value.
![image](https://github.com/user-attachments/assets/de77c8f5-8e00-4c43-a445-a03f7d01a38b)
Below is the residual plots.
![image](https://github.com/user-attachments/assets/bd3b3a44-081e-4a3c-868a-b29cf0c50524)

![image](https://github.com/user-attachments/assets/db186a70-5ac9-4868-aac1-2e6b9b9bc6f7)

## KNN model building 
To predict the species of fish based on its characteristics like height, weight, length.
Data preparation was done so that model can understand the data. 
All the values were standardized on same scale. Data set was randomly partitioned into the ratio of 0.8:0.2.
![image](https://github.com/user-attachments/assets/61688ba1-8b5d-4991-b3c0-67e65eeb1ad8)

![image](https://github.com/user-attachments/assets/01a98397-f935-4ba7-b093-69078d2065c5)
Below confusion matrix, shows the performance of knn model. 
![image](https://github.com/user-attachments/assets/4b1f4b41-35e6-4355-95c9-9ba1f665a7d7)
At k=2, model gave highest accuracy.
![image](https://github.com/user-attachments/assets/84225393-b360-48d9-8b88-acd370c321d5)







