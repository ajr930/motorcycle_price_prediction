# How much should a used motorcylce cost?
![image](https://user-images.githubusercontent.com/83923459/137983629-f53fc9cd-2997-4258-a932-e218f4ce2c4f.png)

# Data-Mining/ Scraping
To obtain our data we scraped over 20,000 listings of motorcycles listed on Craigslist.com in varios major cities to obtain a large sample of data

# Business Problem
The secondary market (Craigslist, Facebook Marketplace, Ebay, etc.. )is completely unregulated and sometimes you want to know if you are overpaying for a product or getting a good deal. 

The item that we are using is motorcycles and to predict how much a used motorcycle should cost we will use many of their features (make, model, odometer, condition, year, etc.. )

# Modeling / Metrics
After our analysis our best model was the XGBoost Regressor.
The metrics we used are R-squard and Root Mean Squared Errot.

# Deployment
Flask app that accepts inputs of the motorcycle features to know in what range we should be paying for a motorcycle
