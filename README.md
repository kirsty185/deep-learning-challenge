# deep-learning-challenge

## Background
The nonprofi t foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the bestchance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use thefeatures in the provided dataset to create a binary classifi er that can predict whether applicants will be successful iffunded by Alphabet Soup.
From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organisations thathave received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capturemetadata about each organisation, such as:
* EIN and NAME
* APPLICATION_TYPE
* AFFILIATION
* CLASSIFICATION
* USE_CASE
* ORGANIZATION
* STATUS
* INCOME_AMT
* SPECIAL_CONSIDERATIONS
* ASK_AMT
* IS_SUCCESSFUL

## Before You Begin
1. Create a new repository for this project called deep-learning-challenge. Do not add this Challenge to an existing repository.
2. Clone the new repository to your computer.
3. Inside your local git repository, create a directory for the Deep Learning Challenge.
4. Push the above changes to GitHub.

## Instructions
### Step 1: Preprocess the Data
Using your knowledge of Pandas and scikit-learn’s StandardScaler(), you’ll need to preprocess the dataset. This step prepares you for Step 2, where you'll compile, train, and evaluate the neural network model.
Using the information we provided in the Challenge fi les, follow the instructions to complete the preprocessingsteps.
1. Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset:
* What variable(s) are the target(s) for your model?
* What variable(s) are the feature(s) for your model?
2. Drop the EIN and NAME columns.
3. Determine the number of unique values for each column.
4. For columns that have more than 10 unique values, determine the number of data points for each unique value.
5. Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variablestogether in a new value, Other , and then check if the binning was successful.
6. Use pd.get_dummies() to encode categorical variables.
7. Split the preprocessed data into a features array, X, and a target array,y. Use these arrays and the
train_test_split function to split the data into training and testing datasets.
8. Scale the training and testing features datasets by creating a StandardScaler instance, fi tting it to the trainingdata, then using the transform function.

### Step 2: Compile, Train, and Evaluate the Model
1. Continue using the Jupyter Notebook in which you performed the preprocessing steps from Step 1.
2. Create a neural network model by assigning the number of input features and nodes for each layer usingTensorFlow and Keras.
3. Create the fi rst hidden layer and choose an appropriate activation function.
4. If necessary, add a second hidden layer with an appropriate activation function.
5. Create an output layer with an appropriate activation function.6.
Check the structure of the model.
7. Compile and train the model.8.
Create a callback that saves the model's weights every fi ve epochs.
9. Evaluate the model using the test data to determine the loss and accuracy.
10. Save and export your results to an HDF5 fi le. Name the fi le
AlphabetSoupCharity.h5.

### Step 3: Optimise the Model
* Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
   * Dropping more or fewer columns.
   * Creating more bins for rare occurrences in columns.
   * Increasing or decreasing the number of values for each bin.
* Add more neurons to a hidden layer.
* Add more hidden layers.
* Use different activation functions for the hidden layers.
* Add or reduce the number of epochs to the training regimen.

### Step 4: Write a Report on the Neural Network Model
The report should contain the following:
1. Overview of the analysis: Explain the purpose of this analysis.
2. Results : Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing
* What variable(s) are the target(s) for your model?
* What variable(s) are the features for your model?
* What variable(s) should be removed from the input data because they are neither targets nor features?

Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
* Were you able to achieve the target model performance?
* What steps did you take in your attempts to increase model performance?

3.Summary: Summarise the overall results of the deep learning model. Include a recommendation for how adifferent model could solve this classifi cation problem, and then explain your recommendation.