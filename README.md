
PREDICTING HOW LIKELY INDIVIDUALS ARE TO RECEIVE H1N1 VACCINE

Introduction

Business Understanding

Problem Statement

Objectives

Data Understanding

Data Preparation

Exploratory Data Analysis

Feature Engineering

Modeling

Feature Selection

Hyperparameter Tuning

Conclusion

Introduction

The 2019 Covid-19 pandemic really shook the world and also shown light on some of the loop holes in the health sector, some of which are vaccination trends and uptake. The prevention of infectious diseases depends heavily on vaccination which is a critical component of public health. But not everyone reacts to immunization in the same way. People react differently, they may experience different side effects such as fever, feel dizzy or soreness. Our objective is to create a reliable classification model that can correctly evaluate a person’s response to h1n1 vaccine based on specific characteristics which are but not limited to age, education and race among others. The end result of this initiative will help healthcare practitioners to make decisions about the delivery of the vaccine. 

Problem Statement

Vaccination has become a key public health measure that is used to fight and in most cases curb infectious diseases. Vaccines provide immunization for individuals and having a community participate in the process can further decrease the spread of diseases as a result of the concept of "herd immunity." The goal of this project is to build a model that can predict the response of individuals to a vaccine based on certain features, such as age, sex, health status, and their knowledge on H1N1 vaccine. This information can help healthcare professionals make informed decisions about who should receive the vaccine and how to best manage its administration.

Objectives

To build a classification model that can predict the reaction of individuals to a vaccine based on certain factors. 
Identify which factors affects individual’s vaccine uptake.
Build a classification model that accurately predicts the response of individuals to new vaccines.

Data Understanding

Data Description

The dataframe has 26707 observations and 35 features. The data on the training features (the input variables that the model will use to predict the probability that people received H1N1 flu vaccines and seasonal flu vaccines) contains 35 feature columns in total, each a response to a survey question.

Data Preparation

The data underwent cleaning and preprocessing processes that would ensure it was in the right form for modeling. This was done dealing with missing values by dropping and filling in. The duplicates were also dropped and categorical data was encoded using label encoding. In EDA trends in the distribution and correlation of the features and the target variable was established.

Modeling

In this section,three models were built. The first was the base model; a logistic regression model that was fitted on the training set before any feature selection was done. Fitting this model to the test data resulted in a very weak f1 score of 42%, and regardless of the contrasting higher accuracy score, the model was considered a poor performing model. For the second model, we built a decision tree that resulted in an f1 score of 52%, still a poor performance. Following the same kind of results after building two models, there was need to do more to improve the outcome. A third model random forest also did well with hyperparameter tuning with an accuracy score of 84%.

Conclusion

After experimenting with different models using different techniques, the final model (the decision tree), which was tuned by hyperparameters was selected. This is because it met the success criteria by recording an accuracy score of 83%. By adjusting the hyperparameters, we were able to find the optimal complexity that balanced overfitting and underfitting.

Recommendation

The public health sector should carry out more research on how people responded to other vaccines because while this model may provide important insight, it may not be as conclusive as a weighted outcome of several different vaccine types.

From evaluating the distribution of H1N1 vaccine, it was established that only around 20% of the individuals had taken the vaccine. The public health organization in charge should look deeper into the reasons behind people not wanting to take the vaccine. It could be that they are not concerned enough, or do not have enough knowledge because it was established during EDA that with increase in levels of concern and knowledge about the vaccine by individuals, the higher the chances were of them taking the vaccine.


For More Information
Notebook https://github.com/pmgitonga/Phase_3_Project/blob/main/Phase_3_Project.ipynb

Presentation https://github.com/pmgitonga/Phase_3_Project/blob/main/Presentation.pdf