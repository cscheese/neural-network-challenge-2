# neural-network-challenge-2
## Module 19 - Neural Networks and Deep Learning Part 2- Challenge 2
#### Due Oct 22, 2024
Carolyn Scheese

### Acknoweldgements
I used Google Colab's AI -Tool to create much of the code within this project (see comments within the code). I found the code to be about 90% correct. I also had two tutoring sessions which helped me correct some code. Finially, I attended before and after class office hours and my instructor, Bill 
was able to identify and help me correct the final piece of code that needed to be fixed. 

### Background and Purpose 
You are tasked with creating a neural network that HR can use to predict whether employees are likely to leave the company. Additionally, HR believes that some employees may be better suited to other departments, so you are also asked to predict the department that best fits each employee. These two columns should be predicted using a branched neural network.

### Files 
https://static.bc-edx.com/ai/ail-v-1-0/m19/lms/datasets/attrition.csv
attrition.ipynb from Module 19

## Import
- from sklearn.model_selection import train_test_split
- from sklearn.preprocessing import StandardScaler
- import pandas as pd
- import numpy as np
- from tensorflow.keras.models import Model
- from tensorflow.keras import layers
- from sklearn.model_selection import train_test_split

### Before you Begin 
- Create a new repository in GitHub called _`neural-network-challenge-2`_
- Add the starter file attrition.ipynb_ from Module 19


### Note
>Although you can use other tools, it is highly recommended you use Google Colab to complete this assignment. Some computers and environments have challenges with tensorflow and tensorflow.keras

### Instructions 
This challenge consists of the following steps:
#### Part 1. Preprocessing
- Import the data and view the first five rows.
- Determine the number of unique values in each column.
- Create y_df with the attrition and department columns.
- Create a list of at least 10 column names to use as X data. You can choose any 10 columns you’d like EXCEPT the attrition and department columns.
- Create X_df using your selected columns.
- Show the data types for X_df.
- Split the data into training and testing sets.
- Convert your X data to numeric data types however you see fit. Add new code cells as necessary. Make sure to fit any encoders to the training data, and then transform both the training and testing data.
- Create a StandardScaler, fit the scaler to the training data, and then transform both the training and testing data.
- Create a OneHotEncoder for the department column, then fit the encoder to the training data and use it to transform both the training and testing data.
- Create a OneHotEncoder for the attrition column, then fit the encoder to the training data and use it to transform both the training and testing data.

#### Part 2. Create, Compile, and Train the Model
- Find the number of columns in the X training data.
- Create the input layer. Do NOT use a sequential model, as there will be two branched output layers.
- Create at least two shared layers.
- Create a branch to predict the department target column. Use one hidden layer and one output layer.
- Create a branch to predict the attrition target column. Use one hidden layer and one output layer.
- Create the model.
- Compile the model.
- Summarize the model.
- Train the model using the preprocessed data.
- Evaluate the model with the testing data.
- Print the accuracy for both department and attrition.

#### Part 3. Summary
Briefly answer the following questions in the space provided:
1. Is accuracy the best metric to use on this data? Why or why not?
2. What activation functions did you choose for your output layers, and why?
3. Can you name a few ways that this model could be improved?
