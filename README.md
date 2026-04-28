# NYC Airbnb Analysis Project

This project analyzes Airbnb listings in New York City using data visualization, data cleaning, and machine learning models to understand and predict listing prices.

The dataset used in this project is the NYC Airbnb 2019 dataset from Kaggle.


## Milestone 1 – Exploratory Data Analysis

This milestone focuses on understanding the dataset through cleaning and visualization.

Tasks completed:

• Data description and assessment  
• Data cleaning and handling missing values  
• Removal of illogical entries such as price = 0  
• Conversion of last_review to datetime format  

Single-variable visualizations:

• Price distribution  
• Room type distribution  
• Number of reviews  
• Availability throughout the year  

Multi-variable visualizations:

• Price vs number of reviews  
• Price by room type and neighbourhood group  

These visualizations helped identify patterns such as highly skewed price distributions and higher average prices in Manhattan compared to other boroughs.


## Milestone 2 – Prediction Models

This milestone builds machine learning models to predict Airbnb listing prices.

Target Variable:

• price (nightly listing price)

### Data Preparation:

• Dummy variables were created for room_type and neighbourhood_group  
• Data was split into training and testing sets (80% training, 20% testing)  
• Extreme price outliers above $1000 were removed to improve model performance  

### Model 1 – Linear Regression

Multiple linear regression models were tested using different sets of predictor variables.

#### Steps included:

• Initial regression model using all variables  
• Removal of variables with high p-values (e.g., neighbourhood_group_Queens)  
• Removal of extreme price outliers  
• Final linear regression model achieved:

R² ≈ 0.313  
Test MSE ≈ 8433  

### Model 2 – Decision Tree Regression

Decision tree models were tested using different maximum depths:

Depth 3  
Depth 5  
Depth 7  
Depth 9  

#### Results showed:

Best Model: max_depth = 7  
Test MSE ≈ 7760 

The decision tree model performed better than linear regression and captured more complex relationships in the data.


### Model Comparison

Linear Regression Test MSE: ~8433  
Decision Tree Test MSE: ~7760  

The decision tree model produced more accurate predictions and was selected as the final recommended model.


## Dataset

NYC Airbnb 2019 dataset  
48,895 listings  
16 columns  

Includes:

• price  
• room type  
• neighbourhood group  
• latitude and longitude  
• number of reviews  
• availability  


## Files in Repository

airbnb_analysis.ipynb – Milestone 1 analysis  
milestone2_models.ipynb – Machine learning models  
dataset.csv – Airbnb dataset  
README.md – Project description  


## Project Webpage

The full analysis, visualizations, and model explanations are available on the project webpage.

Website Link: https://sites.google.com/view/nycairbnbdataanalysis/home


## GitHub Repository

GitHub Repository Link: https://github.com/Mariz133/Airbnb_NYC_Project
