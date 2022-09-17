# Neural_Network_Charity_Analysis

## Overview
Using a CSV from Alphabet Soup containing more than 34,000 organizations that have received funding from Alphabet Soup over the years, a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup will be created.

The analysis will contain:
  - Preprocessing Data for a Neural Network Model
  - Compile, Train, and Evaluate the Model
  - Optimize the Model

## Results
### Data Processing:
- #### What variable(s) are considered the target(s) for your model? 
  - From the dataset IS_SUCCESSFUL is considered as the target for our model.
- #### What variable(s) are considered to be the features for your model?
  - Variables that are features include APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
- #### What variable(s) are neither targets nor features, and should be removed from the input data?
  - EIN and NAME are neither targets nor features so they are dropped from the dataframe.

### Compiling, Training, and Evaluating the Model:
- #### How many neurons, layers, and activation functions did you select for your neural network model, and why? Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
  - Initial Attempt - Using only 2 layers, the target model performance did not reach 75% accuracy.
  ![image](https://user-images.githubusercontent.com/103764279/190876408-738c99a9-d5e6-46d0-ac56-7b490c8e9a36.png)
  ![image](https://user-images.githubusercontent.com/103764279/190876441-a16e9cc2-3b2c-4be7-8830-d8ee2d666799.png)
  - Second Attempt - When adding a third layer, the outcome didn't change and the target model performance did not reach 75% accuracy.
  ![image](https://user-images.githubusercontent.com/103764279/190876535-6e7c2d96-6b5d-460f-8dbc-b7c292f76e65.png)
  ![image](https://user-images.githubusercontent.com/103764279/190876568-b8e25218-d3af-4276-ba4a-09a0a74af65f.png)
  - Third Attempt - Using only 2 layers where layer one had double the amount of neurons as layer two. This attempt was closer to reaching the target model performance, but was still not able to reach the 75% accuracy.
  ![image](https://user-images.githubusercontent.com/103764279/190876647-9447491a-f8d9-485b-a5c5-8404f9a175d2.png)
  ![image](https://user-images.githubusercontent.com/103764279/190876665-99965f76-c943-489d-b63b-8101f7f4897b.png)

## Summary
In three attempts, the model failed for reach the target model performance of 75% accuracy. A recommendation for reaching that accuracy would be to add or gather more data to add to the dataset to make it larger. As complex as the dataset was already, it seems like in order to reach a higher accuracy, a larger dataset could be needed.
