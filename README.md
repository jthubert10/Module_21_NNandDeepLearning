# Project Title

Alphabet Soup Charity

## Overview

In this project, we will preprocess the Alphabet Soup Charity dataset and build a neural network model to predict if an organization will be successful based on the features in the dataset. 

## Preprocessing the Data

### Step 1: Preprocess the Data

1. Read in the charity_data.csv to a Pandas DataFrame.
2. Identify the target variable(s) and feature variable(s) for the model.
3. Drop the EIN and NAME columns.
4. Determine the number of unique values for each column.
5. For columns that have more than 10 unique values, determine the number of data points for each unique value.
6. Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.
7. Use pd.get_dummies() to encode categorical variables.
8. Split the preprocessed data into a features array, X, and a target array, y. Use these arrays and the train_test_split function to split the data into training and testing datasets.
9. Scale the training and testing features datasets by creating a StandardScaler instance, fitting it to the training data, then using the transform function.

### Step 2: Compile, Train, and Evaluate the Model

1. Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.
2. Create the first hidden layer and choose an appropriate activation function.
3. If necessary, add a second hidden layer with an appropriate activation function.
4. Create an output layer with an appropriate activation function.
5. Check the structure of the model.
6. Compile and train the model.
7. Create a callback that saves the model's weights every five epochs.
8. Evaluate the model using the test data to determine the loss and accuracy.
9. Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity.h5.

### Step 3: Optimize the Model

1. Import your dependencies and read in the charity_data.csv to a Pandas DataFrame.
2. Preprocess the dataset as you did in Step 1. Be sure to adjust for any modifications that came out of optimizing the model.
3. Design a neural network model, and be sure to adjust for modifications that will optimize the model to achieve higher than 75% accuracy.
4. Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity_Optimization.h5.

## Technologies Used

- Pandas
- scikit-learn
- TensorFlow
- Keras