# OVERVIEW

In this application, you will explore a dataset from kaggle. The original dataset contained information on 3 million used cars. The provided dataset contains information on 426K cars to ensure speed of processing. Your goal is to understand what factors make a car more or less expensive. As a result of your analysis, you should provide clear recommendations to your client -- a used car dealership -- as to what consumers value in a used car.

# Business Understanding

From a business perspective, we are tasked with identifying key drivers for used car prices. In the CRISP-DM overview, we are asked to convert this business framing to a data problem definition. Using a few sentences, reframe the task as a data task with the appropriate technical vocabulary.

From the original dataset of 3 million used cars identify popular models that customers would be interested in buying and identifying key attributes in the cars that could help the dealerships sell them faster. Shorter time on the lots means lower depreciation of the value and higher profits. selling them quicker frees up space for new inventory allowing the dealership to offer a broader selection of vehicles to their customers based on Market Demand. This also helps dealerships to maintain positive Cash flow by helping them realize faster ROI on each car.

# Data Understanding




# Data Preparation


# Modeling

Below four models were built and evaluated using the GridSearchCV for Cross validation with different hyperparameters.
1. Linear Regression Model
2. Ridge Model
3. Lasso Model
4. Linear Selection Feature Model

The models were built for maximizing the Mean Squared error.

# Evaluation
The above Four models were built with Scoring to Maximize Mean Squared error. Below table captures the data points from these models :

### Model Performance Metrics

| Model                           | Cross Validation Score | Mean Squared Error      |
|---------------------------------|-------------------------|-------------------------|
| Linear Regression Model         | 92,674,643.86           | 92,377,618.22           |
| Ridge Model                      | 92,365,806.74           | 92,071,649.48           |
| Lasso Model                      | 123,640,412.65          | 122,918,402.66          |
| Linear Feature Selection Model  | 105,586,997.59          | 105,219,166.49          |

It is clear that the Ridge model is the best performing model with Linear regression model coming close to second.

# Deployment

Looking at these performing models it is clear that Odometer, Year, Fuel Type, Drive and Condition are the most important features determining the price of the car. Cars with less miles(Odometer) and most recent year models could lead to higher sales.

