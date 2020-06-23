# House-Price-Linear-Regression
## Linear Regression - King County
### Objective
We will be working on a dataset that has sales prices of houses in King County. As a data scientist, you are given a responsibility to create a machine learning model that would predict the sales price for each house in future based on certain input variables. The target variable in this dataset is 'price' and you are given a new unseen test dataset on which you will have to predict price of each house.

### Dataset
You can see the dataset here

To load the dataset in your jupyter notebook, use the below command:
```
import pandas as pd
house_data = pd.read_csv('https://raw.githubusercontent.com/dphi-official/Datasets/master/kc_house_data/kc_house_data.csv')
```
### Data Description
In this dataset the sales price of houses in King County (Seattle) are present. It includes homes sold between May 2014 and May 2015. Before doing anything we should first know about the dataset what it contains what are its features and what is the structure of data.

price: price of the house. This is our target variable.
bedrooms: Number of bedrooms
bathroooms: Number of bathrooms
sqft_living: Square footage of house
sqft_lot: Square footage of lot
floors: Number of floors/ Level
waterfront: 1 = Waterfront view; 0 = No waterfront view
view: 1 = House been viewed; 0 = House has not been viewed
condition: 1 indicates worn out property and 5 excellent
grade: Overall grade given to the housing unit, based on King County grading system. 1 poor ,13 excellent
sqft_above: Square footage of house apart from basement
sqft_below: Square footage of the basement
yr_built: Year of house built
yr_renovated: Year of house renovated
zipcode: Zip code
lat: Latitude coordination
long: Longitude coordination
sqft_living15: Square footage of house in 2015 (implies-- some renovations)
sqft_lot15: Square footage of lot in 2015 (implies-- some renovations)
Evaluation Criteria
Submissions are evaluated on Root-Mean-Squared-Error (RMSE) between the predicted value of your model and true value of sales price on the unseen new test dataset mentioned under submission guidelines below.

## Steps to Build Your Model
Create a linear regression model for target variable 'price'. You can follow the general machine learning model steps as listed under:

Load the necessary libraries such as pandas, numpy, scikit-learn and more if any
Load your dataset and perform exploratory data analysis to identify patterns in the dataset
You may fill mssing values if any (use mode for categorical column and mean/median for numerical columns). If there are no missing values, you may skip this step
Separate Input Variables and Target variable
Split the dataset 'house_data' into train set and test dataset. Now what is this 'house_data'? - don't worry, just scroll up to dataset section above, we have declared the name of our dataset as house_data.
Build a Linear Regression Model
Predict the target variable for your own test dataset created in step 5 and check the model performance
Now, use your model to predict the house price on new test dataset given under the "Submission Guidelines" section.
Once you submit your predictions in precribed format given under "Submission Guidelines" section, you will get a score based on your model performance.
Not happy with your model performance? It is alright, you can try to optimise the model further to improve the performance of your model and submit your predictions again.
Submission Guidelines & Help Documentation
Load the new unseen test data (name it as 'test_new'). You can load the data using the below command.
```
test_new = pd.read_csv('https://raw.githubusercontent.com/dphi-official/Datasets/master/kc_house_data/kc_house_new_test_data.csv')
```
Here the price column is deliberately not there as you need to predict it.

With the model you have built from the earlier section, predict the target variable 'price' on the new unseen test data that you loaded in step 1. Store the predicted values in a variable 'price'

If you are facing challenges to build their model refer to this: https://youtu.be/nsYxsKvtU4A

This dataset earlier appeared on Kaggle (https://www.kaggle.com/harlfoxem/housesalesprediction) and we are using it for learning purpose.
