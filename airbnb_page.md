## Statistical Analysis of Airbnb Rates in New York City ##

### Project description: ### 

When it comes to AirBnb hosting, figuring out realistic and appropriate rates to charge for their listing can be challenging, and oftentimes, AirBnb hosts have little guidance on how to price them. Not knowing how to price listings can lead to oversaturated markets, unreasonabley priced units and a loss of host's profits. Hosts do not want to overcharge because it could lower potential bookings due to lower demand at high price, but at the same time, they do not want to undercharge, because they could not gain expected revenue.

Hosts have to determine a price that is fair to both themselves and their guests. AirBnb pricing is typically influenced by factors including location, number of reviews, room types, and availability.

The goal of the project was to create a forecast model that gives AirBnb hosts an idea of how they should price their listing in response to mentioned factors. With a forecast model, hosts are able to price fairly and make the profit their listing warrants. This forecast model also helps renters get fair prices on the places they are staying.

----
**1. Describe the chosen dataset.**

The goal of the project is to identify the factors that contribute to the price of an Airbnb listing. The New York City Airbnb Open Data dataset was chosen to be used for the project. The data resource is from Kaggle database, with a CSV Airbnb data set gathered by dgomonov in 2019. In addition, to be an appropriate dataset for the project, the data was free to access and could easily be imported into Jupyter. This dataset provides qualitative and quantitative details about Airbnb units in the chosen location of the project, New York City. The information of the dataset will allow for the analysis of prices of units in terms of various factors such as locations, number of reviews, room types, and availability to allow hosts to more appropriately price units according to current market rates. New York City was chosen due to its competitive nature, oversaturation, and high prices of Airbnb listings. The prices and saturation in New York reflect similar trends that are beginning to be seen in several cities across the country. The results found from this dataset can be used for future predictions and trends in other locations.

---
**2. Explain your model and all the steps involved in your modeling.**

First, the independent and dependent variables were identified. The independent variables were neighborhood_group, neighborhood, latitude, longitude, room_type, minimum_nights, number_of_reviews, reviews_per_month, calculated_host_listings_count, and availability_365. The only dependent variable was the price.

Then, the dataset was split into training and testing sets. 80% of the data was training and the remaining 20% was for testing. The data was split into testing and training to measure the overall accuracy.

Finally, linear regression and random forest models were implemented. Both models were used in this project since the team wanted to see which model can bring out better result. The coefficient of determination R^2 on test set and train set were then calculated for both models. The closer R^2 to 1, the better the model performs.

---
**3. Explain clearly the results (outcomes) of your project.**

The random forest model was able to predict Airbnb rates with the accuracy of 87%. The model did a great job forecasting less expensive listings. However, the more expensive the listing got, the harder it was for the model to predict. This could be due to the fact that the dataset didn't have as many expensive listings compared to less expensive listing. Therefore, the model didn't have enough data points to learn the pattern of expensive Airbnb rates.

---
**4. Explain performance analysis to justify your results.**

After performing both linear regression and random forest, the linear regression model yielded 6% accuracy while the random forest model yielded 87%. Random forest model definitely gave much higher accuracy. It is because a prediction from the random forest regressor is an average of the predictions produced by the trees in the forest, while linear regression is just simply a linear model that only works well with linear-shape data. Additionally, random forest has much more parameters compared to linear regression. These features of random forest helps the model produce higher accuracy in terms of prediction.

---
**5. Explain the conclusions.**

The features importance bar graph shows which factors have heavy influences on NYC Airbnb pricing. Surprisingly, longitudes and latitudes showed higher importance in pricing determination, despite the team's expectation of neighbourhood groups. This could be explained by the fact that each neighbourhood group or borough has its own downtown, and when tourists visiting that borough, they tend to be drawn to stay near downtown due to closer tourist attractions and easier and shorter commute between destinations. Thus, the location of Airbnb in each borough, closer to downtown or not, is an important factor when defining the pricing rate.

---
**6. Three real world use cases of your project**

This project can determine how to price an Airbnb appropriately given relevant and current information of the New York City area. A new Airbnb provider in the New York City area can reference these materials to determine how much to charge a tenant for their stay. Also, a tenant looking to stay in the New York City area can use these materials and determine whether they are being charged appropriately. Lastly, local communities can determine how much their community is worth in terms of visiting desirability as to determine how much to invest in the local tourism and accommodations.
