# Car Advert Dataset Price Analysis and Prediction (AutoTrader Car Advert Dataset Price Analysis)
### By Anthony Eze

### Introduction
Car Advert Dataset Price Analysis and prediction: I will be working with a dataset provided by AutoTrader, which contains anonymized car sale adverts with information on various features such as brand, type, color, mileage, and selling price. My task is to perform a structured set of tasks to uncover interesting associations and group differences that have a significant impact on the valuation of vehicles. I am looking forward to using my knowledge and skills in data understanding, exploration, preparation, and hypothesis testing to uncover valuable insights from this dataset. I am eager to dive into the world of data science and see what insights I can uncover from this dataset. The Dataset originally contained more than 400,000 but i am working with a sampled 200,000 rows.

Some of the questions to answer from the analysis

 - What's the correlation between the price and other features? What feature influences the price of cars?
 - Does mileage impact the value of cars?
 - What is the average price of vehicles by body type?
 - what is the average price of vehicles by fuel_type?
 - Does the year of registration affect the average price?

### Preliminary Data Wrangling
The following actions have to be performed on the dataset to prepare it for analysis:

 - Drop the public reference column
 - Deal with the missing values in the following column - year_of_registration
 - Drop the NEW cars in the vehicle_condition which effectively drops the entire column
 - Deal with the missing values in the following columns - reg_code
 - Deal with the missing values in the following columns mileage, standard_colour, body_type, and fuel_type
 - Deal with error values in year of registration column e.g 999
 - Detecting outliers using interquatile range and dropping all outliers from the dataset

### Preliminary Data Transformation 
 The following data transformation can be performed on the dataset columns:
 
 - Calculating the age of the vehicle based on the current date and the year of registration
 - Creating categorical variable from year of registration column
 - Creating categorical variable from mileage column

### Summary of Findings
From the analysis, below are some of the findings as related to the main features:

Exploring the data gave us some insight into the data as we compared some of the variables to the car advert dataset.

Variables such as mileage', 'standard_colour', 'standard_make','standard_model', 'vehicle_condition', 'year_of_registration', 'crossover_car_and_van', 'fuel_type' are the independent variables and 'price' is the dependent variable.

From the analysis: 

1. Correlation Summary
<br>

**'price' vs 'year_of_registration'**
- There is a strong positive correlation between price and year_of_registration.
- As the value of year_of_registration increases, there is a strong tendency for the price to increase.
- A correlation coefficient of 0.62 is relatively large and suggests that year_of_registration is a very good predictor of price.
<br>

**'price' vs 'mileage'**
- There is a moderate negative correlation between price and mileage.
- As the value of mileage increases, there is a tendency for the price to decrease.
- A correlation coefficient of -0.51 is relatively moderate and suggests that mileage is a fairly good predictor of price, but not as strong as year_of_registration.
<br>

**'price' vs 'age'**
- There is a strong negative correlation between price and age.
- As the value of age increases, there is a strong tendency for the price to decrease.
- A correlation coefficient of -0.62 is relatively large and suggests that age is a very good predictor of price.
<br>

**'price' vs 'crossover_car_and_van'**
- There is a weak positive correlation between price and crossover_car_and_van.
- As the value of crossover_car_and_van increases, there is a slight tendency for the price to increase as well, but the relationship is not very strong.
- A correlation coefficient of 0.05 is relatively low and suggests that crossover_car_and_van is not a very good predictor of price.

2. Mileage relationship with price
<br>

- It appears that as mileage increases, the price of the car decreases. This is likely due to the fact that cars with higher mileage have been used more and may have more wear and tear, making them less valuable. Additionally, the plot shows that cars with low mileage and cars that are new have relatively higher prices compared to cars with average and high mileage. This could be because new cars and cars with low mileage are considered more desirable and therefore command a higher price.

3. Body type relationship with price
<br>

- From these results, we can infer that the most common body types are Hatchback, SUV, and Saloon. The body types with the highest mean prices are Camper, Chassis Cab, and Minibus, which suggests that these are likely to be more expensive types of vehicles. The body type with the lowest mean price is Hatchback, which suggests that this is likely to be a more affordable type of vehicle.
<br>

- Overall, these results can provide insights into the market demand for different types of vehicles and can be useful for car manufacturers and dealerships in determining their pricing and marketing strategies.

4. Fuel type relationship with price
<br>

- We can see that the average price of cars with diesel plug-in hybrid fuel type is the highest followed by diesel hybrid and petrol plug-in hybrid. The average prices of electric and petrol hybrid cars are also relatively high. On the other hand, the average prices of cars with petrol and bi-fuel are the lowest.
<br>

- we can infer that people who are willing to spend more on cars tend to choose plug-in hybrids, diesel hybrids, and electric cars. This might be because these types of cars are more environmentally friendly and have lower fuel costs in the long run. On the other hand, people who prioritize affordability and convenience may opt for petrol and bi-fuel cars. However, it's important to note that the choice of fuel type may also be influenced by factors such as availability, government regulations, and personal preferences.

5. Year of registration relationship with price
<br>

- As the year of registration goes further back in time, the average price of cars decreases. This can be attributed to factors such as wear and tear, newer and more advanced models, and changes in market demand. This information can help in determining the value of a car and can be useful for individuals looking to sell their car or car dealerships to set a fair price based on the year of registration.
<br>

- From this analysis, we can infer that the year of registration does affect the average price of cars. Generally, newer cars tend to have a higher price compared to older cars. However, there may be exceptions to this trend, such as classic or vintage cars that may have a higher price due to their rarity or unique features.



### Limitations on the project
1. Quality of data: The accuracy and completeness of the data can be a limitation. If there are missing values or errors in the data, it can affect the quality of the analysis and the conclusions drawn from it.

2. Representativeness of the sample: The dataset might not be a representative sample of the entire population of cars. For example, the dataset might overrepresent certain brands or models of cars, making it difficult to generalize the results to the entire population.

3. Time period: The data might not be up-to-date, or it might not cover a long enough time period to capture changes in the market over time.

4. Data bias: There might be biases in the data collection process that could impact the analysis. For example, if the data was collected from a specific region, it might not be applicable to other regions.

5. Confounding variables: There might be other variables that are not included in the dataset that could affect the relationship between car features and prices. For example, the dataset might not include variables such as fuel prices or economic indicators that could impact car prices.
<br>

It's important to consider these limitations when analyzing the dataset and drawing conclusions from it.
