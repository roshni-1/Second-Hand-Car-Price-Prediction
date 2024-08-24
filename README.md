# Objective:
 The objective of the "Second-hand Car Price Prediction" project is to develop a machine learning model capable of accurately predicting the price of second-hand cars based on various features and specifications of the vehicles.
 
**Datasource:** https://www.kaggle.com/datasets/sujithmandala/second-hand-car-price-prediction 


**Steps Taken**
- Reading the data in python
- Defining the problem statement
- Identifying the Target variable
- Looking at the distribution of Target variable
- Basic Data exploration
- Visual Exploratory Data Analysis for data distribution (Histogram and Barcharts)
- Feature Selection based on data distribution
- Detecting and removing outliers, handling missing values.
- Visual correlation analysis
- Statistical correlation analysis (Feature Selection)
- Converting data to numeric for ML
- Sampling and K-fold cross validation
- Trying multiple Regression algorithms
- Selecting the best Model
- Deploying the best model in production

# The features available in the dataset are:-

- **Car_ID:** A unique identifier for each car listing.
- **Brand:** The brand or manufacturer of the car (e.g., Toyota, Honda, Ford, etc.).
- **Model:** The model of the car (e.g., Camry, Civic, Mustang, etc.).
- **Year:** The manufacturing year of the car.
- **Kilometers_Driven:** The total kilometers driven by the car.
- **Fuel_Type:** The type of fuel used by the car (e.g., Petrol, Diesel, Electric, etc.).
- **Transmission:** The transmission type of the car (e.g., Manual, Automatic).
- **Owner_Type:** The number of previous owners of the car (e.g., First, Second, Third).
- **Mileage:** The fuel efficiency of the car in kilometers per liter.
- **Engine:** The engine capacity of the car in CC (Cubic Centimeters).
- **Power:** The maximum power output of the car in bhp (Brake Horsepower).
- **Seats:** The number of seats available in the car.
- **Price:** The selling price of the car in INR (Indian Rupees), which is the target variable to predict.

# Project Steps

1. Data Import and Preprocessing
Data Loading: The dataset containing information on second-hand cars is loaded into a Pandas DataFrame.
Data Cleaning: Missing values are handled, and irrelevant columns are removed. Columns like 'Mileage' and 'Engine' are converted from strings to numerical values for proper analysis.

2. Exploratory Data Analysis (EDA)
Univariate Analysis: Distribution of individual features, such as 'Price,' 'Year,' and 'Kilometers Driven,' is visualized using histograms.
Bivariate Analysis: Relationships between the target variable (Price) and predictor variables like 'Year,' 'Fuel_Type,' and 'Seller_Type' are explored using scatter plots, box plots, and correlation matrices.

3. Feature Selection
Bi-Variate Analysis: The relationship between the continuous target variable (Price) and continuous/categorical predictors is explored using scatter plots, ANOVA tests, and correlation matrices. This helps in selecting features strongly correlated with the target.

4. Model Building
Model Selection: The notebook applies multiple machine learning models, including Linear Regression and Decision Tree, to predict car prices.
Training and Testing: The dataset is split into training and testing sets. Models are trained on the training data and evaluated on the testing data.
Cross-Validation: 10-fold cross-validation is used to validate the model's performance across different data subsets.

5. Model Evaluation
Error Calculation: The Mean Absolute Percentage Error (MAPE) is calculated to assess the accuracy of predictions. The Decision Tree model, though accurate, shows signs of overfitting.
Final Model Selection: Despite the Decision Tree model's high accuracy, the project opts for the Linear Regression model due to its better generalization.

6. Conclusion
Key Findings: The features 'Power,' 'Kilometers Driven,' and 'Engine' are identified as the top predictors of car price. The project concludes with the selection of a Linear Regression model for predicting second-hand car prices.
This comprehensive workflow outlines how the project systematically approaches the problem of predicting second-hand car prices by using machine learning techniques. ​
