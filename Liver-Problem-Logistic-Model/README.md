# Liver Patients - Logistic Regression
## Objective
Patients with liver disease have been continuously increasing because of excessive consumption of alcohol, inhale of harmful gases, intake of contaminated food, pickles and drugs. In an effort to reduce burden on doctors, the government has hired you as a data scientist to build a predictive machine learning that would give an indication whether a person would have liver problem or not. Now, as a data scientist, your goal is to build a logistic machine learning model that predicts whether a patient is healthy (non liver patient) or ill (liver patient) based on some clinical and demographic features (or input variables) listed in the 'Data Description' section.

## Dataset & Data Description
This data set contains liver patient records and non liver patient records collected from North East of Andhra Pradesh, India. The "Liver_Problem" column is the target variable used to divide groups into liver patient ( Liver_Problem == 1) or not ( Liver_Problem == 2).

Liver_Problem == 1, implies the individual is a liver patient
Liver_Problem == 2, implies the individual is not a liver patient
To load the dataset in your jupyter notebook, use the below command:
```
import pandas as pd
liver_data = pd.read_csv('https://raw.githubusercontent.com/dphi-official/Datasets/master/liver_patient_data/indian_liver_patient_dataset.csv')
```

## Data Description:

Age of the patient
Gender of the patient
Total Bilirubin
Direct Bilirubin
Alkaline Phosphotase
Alamine Aminotransferase
Aspartate Aminotransferase
Total Protiens
Albumin
Albumin and Globulin Ratio
"Liver_Problem" column is the target variable used to divide groups into liver patient (liver disease) or not (no disease).
Some of the data are slightly technical, you may refer online resources to learn more about them.

## Steps to Build Your Model
Create a logistic regression model for target variable Liver_Problem. You can follow the general machine learning model steps as listed under:

Load the necessary libraries such as pandas, numpy, scikit-learn and more if any
Load your dataset and perform exploratory data analysis to identify any patterns in the dataset
You may fill mssing values if any (use mode for categorical column and mean/median for numerical columns). If there are no missing values, you may skip this step
Separate Input Variables and Target variable
Split the dataset liver_data into train set and test dataset. Now what is this liver_data? - don't worry, just scroll up to dataset section above, we have declared the name of our dataset as liver_data.
Build a Logistic Regression Model
Predict the target variable for your own test dataset created in step 5 and check the model performance
Now, use your model to predict whether a patient is ill (Liver_Problem == 1) or healthy (Liver_Problem == 2) based on some clinical and demographic features
Not happy with your model performance? It is alright, you can try to optimise the model further to improve the performance of your model and submit your predictions again.

Load the new unseen test data (name it as 'test_new'). You can load the data using the below command.
``` test_new = pd.read_csv('https://raw.githubusercontent.com/dphi-official/Datasets/master/liver_patient_data/indian_liver_patient_new_testdataset.csv') ```
Here the Liver_Problem column is deliberately not there as you need to predict it.

With the model you have built from the earlier section, predict the target variable Liver_Problem on the new unseen test data that you loaded in step 1. Store the predicted values in a variable Liver_Problem

If you are facing challenges to build their model refer to this: https://youtu.be/nsYxsKvtU4A

## Acknowledgements
This dataset was downloaded from the UCI ML Repository:
This was an exercise of 5-week Dphi Data Science Bootcamp.
Lichman, M. (2013). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

Inspiration: Use these patient records to determine which patients have liver disease and which ones do not.
