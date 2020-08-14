# flight-price-prediction
Here im creating a model which will predict price of  flight price , it is regression problem under which im using random regressor 
# Aim
To find best price of flight
# Data
flight data is downloaded from Kaggle
# Procedure
As we know that the price of anything depends on very different different factors, this flight price prediction ,here numbers of flights are present with different route
with different date and time, with the help of one hot encoding i have seprated airline , source, destination and reprensented into one hot encoder and with ordinal ecoding


i have given some order to different differents route {"non-stop": 0, "1 stop": 1, "2 stops": 2, "3 stops": 3, "4 stops": 4}

further using pandas date time module to covnverting whole time into seprate values like (Dephour	Depmin	Arrivalhour	Arrivalmin) and (Journeyday	Journeymonth)


finally after data pre processing steps in train and test data , i have converted whole test and train into numerical form for better approach towards price 
by using EXTRA TREE REGRESSOR find the best or important features for prediction na dthe most important feature i get is total no of stops whcih is converted by ordinal method
and at last connecting all data pipelines and fitting into RANDOM FOREST REGRESSOR and getting accuracy about 69 % which is not good for a model , 


so i start hyper paramter tunning of model and after which i get 79 % accuracy which is 10% more thna previous one

# Python libraries used



      import pandas as pd 
      from sklearn.metrics import confusion_matrix
      from sklearn.metrics import r2_score
      import numpy as np
      import matplotlib.pyplot as plt
      import seaborn as sns
      from sklearn.model_selection import train_test_split
      from sklearn.ensemble import ExtraTreesRegressor
      from sklearn.ensemble import RandomForestRegressor
      from sklearn.model_selection import RandomizedSearchCV 
      from sklearn.model_selection import RandomizedSearchCV 
      
 # Conclusion
 detailed conclusion has been provided in the model fitting RANDOMFORESTREGRESSOR.ipynb
