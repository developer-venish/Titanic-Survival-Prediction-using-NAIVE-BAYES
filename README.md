## Titanic-Survival-Prediction-using-NAIVE-BAYES
ML Python Project

---------------------------------------------------------------------------------------
# Preview
![](https://github.com/developer-venish/Titanic-Survival-Prediction-using-NAIVE-BAYES/blob/main/demo.png)

---------------------------------------------------------------------------------------

All the code in this project has been tested and run successfully in Google Colab. I encourage you to try running it in Colab for the best experience and to ensure smooth execution. Happy coding!

---------------------------------------------------------------------------------------
This code performs the following steps:

1. Install the pandas library using pip and import the necessary libraries: pandas, numpy, and files from google.colab.
2. Upload the 'titanicsurvival.csv' file using the files.upload() function.
3. Read the CSV file into a pandas DataFrame called 'dataset'.
4. Print the shape of the dataset (number of rows and columns) using dataset.shape.
5. Print the first 5 rows of the dataset using dataset.head(5).
6. Convert the 'Sex' column in the dataset to numeric values, where 'female' is mapped to 0 and 'male' is mapped to 1.
7. Print the first 5 rows of the modified dataset to verify the changes.
8. Separate the independent variables (X) from the dependent variable (Y) by dropping the 'Survived' column from X.
9. Fill any missing values in the 'Age' column of X with the mean age.
10. Split the dataset into training and testing sets using train_test_split from sklearn.model_selection.
11. Create an instance of the Gaussian Naive Bayes classifier and fit it to the training data.
12. Take input from the user for a new person's class number, gender, age, and fare.
13. Create a list 'person' with the input values.
14. Use the trained model to predict the survival outcome for the new person.
15. Print the predicted result, indicating whether the person might have survived or not.
16. Predict the survival outcome for the testing data (X_test) and stack the predicted values (Y_pred) with the actual values (Y_test).
17. Calculate and print the accuracy of the model using the accuracy_score metric.

Overall, this code performs data preprocessing, trains a Naive Bayes classifier on the Titanic survival dataset, and allows you to input new person details to predict their survival outcome. It also evaluates the accuracy of the model on the testing data.

---------------------------------------------------------------------------------------
The Gaussian Naive Bayes classifier is a probabilistic machine learning algorithm used for classification tasks. It is based on the Bayes' theorem with the assumption of independence between features. "Gaussian" refers to the assumption that the features follow a Gaussian distribution (also known as normal distribution).

The classifier calculates the probability of an instance belonging to each class based on the observed feature values. It assumes that each class is characterized by a mean vector and a covariance matrix for the feature variables, assuming a Gaussian distribution for each class. Using these probabilities, it assigns the class label that has the highest probability.

The algorithm is called "Naive" because it assumes that the presence of a particular feature in a class is independent of the presence of other features. Although this assumption may not hold in real-world scenarios, the algorithm can still provide reasonable results in many cases and is computationally efficient.

Gaussian Naive Bayes is commonly used for classification tasks where the features are continuous or approximately follow a Gaussian distribution. It has been successfully applied to various domains, including text classification, spam detection, medical diagnosis, and more.

---------------------------------------------------------------------------------------
