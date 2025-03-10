# 21_deep-learning-challenge

# Deliverable(s)
[Report](https://github.com/wrighang/21_deep-learning-challenge/blob/main/neural_report.md)

[alphabet_soup_charity.ipynb](https://github.com/wrighang/21_deep-learning-challenge/blob/main/alphabet_soup_charity.ipynb) ,
[AlphabetSoupCharity.h5](https://github.com/wrighang/21_deep-learning-challenge/blob/main/AlphabetSoupCharity.h5)<br/>

[alphabet_soup_charity_optimization_1.ipynb](https://github.com/wrighang/21_deep-learning-challenge/blob/main/alphabet_soup_charity_optimization_1.ipynb) ,
[AlphabetSoupCharity_Optimization_1.h5](https://github.com/wrighang/21_deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization_1.h5)<br/>
[alphabet_soup_charity_optimization_2.ipynb](https://github.com/wrighang/21_deep-learning-challenge/blob/main/alphabet_soup_charity_optimization_2.ipynb) , 
[AlphabetSoupCharity_Optimization_2.h5](https://github.com/wrighang/21_deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization_2.h5)<br/>
[alphabet_soup_charity_optimization_3.ipynb](https://github.com/wrighang/21_deep-learning-challenge/blob/main/alphabet_soup_charity_optimization_3.ipynb) , 
[AlphabetSoupCharity_Optimization_3.h5](https://github.com/wrighang/21_deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization_3.h5)


## Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received access to a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

`EIN and NAME` —Identification columns
`APPLICATION_TYPE` —Alphabet Soup application type
`AFFILIATION` —Affiliated sector of industry
`CLASSIFICATION` —Government organization classification
`USE_CASE` —Use case for funding
`ORGANIZATION` —Organization type
`STATUS` —Active status
`INCOME_AMT` —Income classification
`SPECIAL_CONSIDERATION` —Special considerations for application
`ASK_AMT` —Funding amount requested
`IS_SUCCESSFUL` —Was the money used effectively

## Requirements
### Preprocess the Data

- Create a dataframe containing the `charity_data.csv` data, and identify the target and feature variables in the dataset.
- Drop the `EIN` and `NAME` columns.
- Determine the number of unique values in each column.
- For columns with more than 10 unique values, determine the number of data points for each unique value.
- Create a new value called `Other` that contains rare categorical variables.
- Create a feature array `X` and a target array `y` by using the preprocessed data.
- Split the preprocessed data into training and testing datasets.
- Scale the data by using a `StandardScaler` that has been fitted to the training data.

### Compile, Train, and Evaluate the Model

- Create a neural network model with a defined number of input features and nodes for each layer.
- Create hidden layers and an output layer with appropriate activation functions.
- Check the structure of the model.
- Compile and train the model.
- Evaluate the model using the test data to determine the loss and accuracy.
- Export the results to an HDF5 file named `AlphabetSoupCharity.h5`.

### Optimize the Model

- Repeat the preprocessing steps in a new Jupyter notebook.
- Create a new neural network model, implementing at least three model optimization methods.
- Save and export the results to an HDF5 file named `AlphabetSoupCharity_Optimization.h5`.

### Write a Report on the Neural Network Model

- Write an analysis that includes a title and multiple sections, labeled with headers and subheaders.
- Format images in the report so that they display correctly.
- Explain the purpose of the analysis.
- Answer all six questions in the results section.
- Summarize the overall results of the model.
- Describe how a different model could be used to solve the same problem, and explain why that model would be chosen.

====================================================================
## CODING_PROCESS

- Referenced module activities throughout the challenge along with class presentation slids. 
