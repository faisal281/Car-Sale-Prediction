This dataset contains information about used cars.
This data can be used for a lot of purposes such as price prediction to exemplify the use of linear regression in Machine Learning.
The columns in the given dataset are as follows:

name,
year,
selling_price,
km_driven,
fuel,
seller_type,
transmission,
Owner

AIM: To predict the Car Sale price

Jobs Done on Data: 
1. Importing the Data
2. Cleaning the data
3. Data Visualization
4. Building the ML model for predicting the price


Importing the Data: Firstly the dataset has been imported in the jupyter notebook.The dataset is relativel small.The data contains the information of cars from past few years based upon which the model has to be built for predicting the prices of the cars.This contain around 301 rows and 9 columns.

Cleaning the Data: Upon looking the data,its has been very clear that the data doesnt contain any null values in it.There were no outliers present as well. But there was categorical data in it which has to be encoded into numerical data. By using pd.get_dummies the categorical features has converted into Numerical.
I added "Current_year" column in the dataset so that,I can subtract it from "Years" so that I can understand and mention how old the car is which inturn help the Model to calculate how old the car is and it can predict it verywell.

Data Visualization: By using the Correlation Heatmap and Pairplot we can easily visulaise how well the features are correlated with eachother and the relationship between the features. This step is the important part so that any user can understand the data verywell.

Building ML model: Random Forest: I have use RandomisedsearchCV for the model and I have used iteration to be 10,verbose to be 2 and for calculating scoring,negative mean square error is used.The data has been split into test and train so that I can fit the model.As it is very clear that upon drawing  the distribution plot it is out to be Gaussian distributed plot.
