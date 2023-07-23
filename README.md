# Bike-sharing-demand-Prediction

almabetter project.

Rental bikes have become increasingly popular in urban cities, offering enhanced mobility comfort. The key to ensuring a smooth experience for the public is making rental bikes readily available and accessible at all times, reducing waiting times. However, one major challenge lies in maintaining a stable supply of rental bikes throughout the city. To address this concern, accurate predictions of the required bike count at each hour are crucial.In this data analysis project, we started by importing the necessary libraries and examining our dataset, which contains 8760 rows and 14 columns, with no duplicate or missing data.

After initial exploration, we focused on studying the individual features and the data they represent. We noticed that the 'Date' column was in 'object' datatype, so we converted it to the datetime datatype. From this column, we extracted additional features such as 'Date', 'month', 'year', and the number of weeks. Subsequently, we dropped the original 'Date' column and renamed certain columns for convenience.

Next, we proceeded with data visualization, creating various charts and graphs to gain useful insights. Based on the visualizations, we formulated three hypothetical statements and performed hypothesis tests to validate them. The statements were:

The average bike count in Seoul city at any point in time is greater than 100.
The average temperature in Seoul city at any point is greater than 10 degrees Celsius.
The standard deviation of humidity in Seoul city is 20.
Following the exploratory data analysis, we addressed some data preprocessing steps. We performed one-hot encoding on categorical features while dropping the first column to avoid multicollinearity. To deal with the right-skewed distribution of the dependent variable 'Rented_bike_count,' we applied a square root transformation to achieve a more normal distribution. Additionally, we used MinMax scaling to scale our features. Finally, we split the data into an 80-20 train-test ratio for model training and evaluation.

Moving on to the machine learning phase, we implemented various models and calculated various statistical parameters to assess their performance. After comparing the models, we found that the Random Forest Regressor exhibited the best performance in predicting the demand for city bikes for a particular hour.

In conclusion, deploying the Random Forest Regressor model can significantly help the bike rental company accurately predict the bike demand, enabling them to efficiently meet the city's bike rental needs.
