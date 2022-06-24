# User-Engagement-Prediction

## Hackathon Solution Approach
## By Gaurav Thakur


### Process Steps
* Data Acquisition
* Data Preprocessing
* Model Selection
* Model Training
* Model evaluation
* Predictions


### Data Acquisition
* Platform - Google colab
* Import required libraries.
* Mount the drive and import the training and test datasets


### Data Preprocessing
* No missing values.
* Drop columns which are unique and can’t get used as independent variables
(row_id,video_id)
* Encoding-
* Label encoding on gender and profession columns for Random Forest Regression


### Model Selection
Models implemented:
* Linear regression and polynomial regression
* One hot encoding on gender and profession.
* Dropped user_id and category_id
* Decision Tree
* Label encoding on gender and profession
* Max_depth = 200
* Random Forest
* Label encoding on gender and profession
* N_estimators = 1000
* GBM
* Label encoding on gender and profession
* N_estimators = 1000
* max_depth=10,min_samples_split= 4,learning_rate= 0.05,random_state=0

## Chosen model is random forest.
#### Though r2 score of GBM was more than Random forest but random forest showed better
result with test data on submission

## Model Training
* Model used- Random Forest Regressor
* N_estimators = 1000, random state = 0
* Train the model on training dataset and use the model for predicting test data results.

## Model Evaluation metrics
#### r2_score_splittedtest= 0.45308118325154545

## Result
* Implement the model on test data to get the results.
* Convert the result into the required format of csv file having two columns - row_id and
engagement_score.
* Upload the predictions on drive
