
# Neural Network Model Report
## Overview
The objective of this analyis is to create a tool for Alphabet Soup that will help determine what charity applications would be successful if funded by Alphabet Soup. This datasset includes historical data containing more than 34,000 organizations that have received funding from Alphabet Soup. 
 
## Results

### Data Preprocessing

***What variable(s) are the target(s) for your model?***
#### 1 Target Value
- `IS_SUCCESSFUL` — Was the money used effectively

***What variable(s) are the features for your model?***
#### 9 Features
- `APPLICATION_TYPE` — Alphabet Soup application type
- `AFFILIATION` — Affiliated sector of industry
- `CLASSIFICATION` — Government organization classification
- `USE_CASE` — Use case for funding
- `ORGANIZATION` — Organization type
- `STATUS` — Active status
- `INCOME_AMT` — Income classification
- `SPECIAL_CONSIDERATION` — Special considerations for application
- `ASK_AMT` — Funding amount requested

***What variable(s) should be removed from the input data because they are neither targets nor features?***
#### Non-beneficial columns
- `EIN and NAME` —Identification columns

### Compiling, Training, and Evaluating the Model

***How many neurons, layers, and activation functions did you select for your neural network model, and why?***
- Initial Model<br/>
Layer 1: 8 neaurons (relu)<br/>
Layer 2: 5 neurons (relu)<br/>
Output: (sigmoid)<br/>
application_type_counts<10<br/>
class_counts<10<br/>
Epochs: 100<br/>
Loss: .5511<br/>
Accuracy: .7290<br/>

- Optimized 1 Model<br/>
Layer 1: 26 neaurons (relu)<br/>
Layer 2: 16 neurons (relu)<br/>
Output: (sigmoid)<br/>
application_type_counts<10<br/>
class_counts<10<br/>
Epochs: 100<br/>
Loss: .5541<br/>
Accuracy: .7269<br/>

- Optimized 2 Model <br/>
Layer 1: 10 neaurons (relu)<br/>
Layer 2: 10 neurons (relu)<br/> 
Layer 3: 5 neurons (relu)<br/>
Output: (sigmoid)<br/>
application_type_counts<10<br/>
class_counts<10<br/>
Epochs: 50<br/>
Loss: .5515<br/>
Accuracy: .7352<br/>

- Optimized 3 Model <br/>
'activation': 'sigmoid',<br/>
 'first_units': 1,<br/>
 'num_layers': 4,<br/>
 'units_0': 6,<br/>
 'units_1': 11,<br/>
 'dropout_rate': 0.30000000000000004,<br/>
 'units_2': 11,<br/>
 'units_3': 26,<br/>
 'units_4': 1,<br/>
 'units_5': 1,<br/>
 'tuner/epochs': 20,<br/>
 'tuner/initial_epoch': 7,<br/>
 'tuner/bracket': 1,<br/>
 'tuner/round': 1,<br/>
application_type_counts<10><br/>
class_counts<10<br/>
Epochs: 50<br/>
Loss: .5710<br/>
Accuracy: .7348<br/>

***What steps did you take in your attempts to increase model performance?***
By the third optimized model I used kerastuner to search for the best hyperparameters added the dropout technique to prevent overfitting the training data by dropping out a fraction of the units in a layer when fitting the model. 

***Were you able to achieve the target model performance?***
No, despite many optimization attempts, including adjustments made outside of what is reported in this assignment, I was unable to reach the target performance of 75%. I achieved an accuracy rate of 73.5%.

## Summary

While the deep learning model did not achieve the target performance of 75%, performance improved from the initial 72.9% with the last attempt at 73.5%. Exploring a different model such as Random Forest could be beneficial. Random Forest is effective in handling complex, non-linear relationships and may yield improved predictions performance. 