# How much should a used motorcylce cost?
![image](https://user-images.githubusercontent.com/83923459/137983629-f53fc9cd-2997-4258-a932-e218f4ce2c4f.png)

# Data-Mining/ Scraping

I obtained my data set from Craigslist by scraping thousands of indivdual listins from major cities across the United States.
With each individual listing I was able to obtain the year the motorcycle was made and the company that produced the motorcycle.
This dataset that the model was trained on was over 20,000 rows of datapoints.
For many of the listings I was able to obtain features that will help with price prediction (odometer reading, condition, fuel type, etc..)


# Business Problem
The secondary market (Craigslist, Facebook Marketplace, Ebay, etc.. )is completely unregulated and sometimes you want to know if you are overpaying for a product or getting a good deal. 

The item that we are using is motorcycles and to predict how much a used motorcycle should cost we will use many of their features (make, model, odometer, condition, year, etc.. )


# EDA
For visualization I used the median price of the motorcycle grouped by the make of the motorcycle.
![image](https://user-images.githubusercontent.com/83923459/138173502-1eee8961-37eb-4e6d-a47a-9d64b011478f.png)

I also did a jointplot on the discribution of the price of motorcycles by year. The higher the price typically means the more recent year but just because it is a more recent year does not mean it is a higher price.
![image](https://user-images.githubusercontent.com/83923459/139141809-3ef1ec03-11c2-49a4-9f33-d89fbc1bf67f.png)



# Modeling / Metrics
After our analysis our best model was the XGBoost Regressor.
The metrics we used are R-squard and Root Mean Squared Error.
We have an R-Squared of 70% and RMSE of $2,556

# Deployment
Flask app that accepts inputs of the motorcycle features to know in what range we should be paying for a motorcycle
![image](https://user-images.githubusercontent.com/83923459/138173642-7956d9cd-e986-4ef8-8002-8b6513536345.png)

