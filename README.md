# ForecastIQ-Predictive-Analytics-for-Sales



 PROBLEM STATEMENT FOR FUTURE SALES PREDICTION:

"The problem at hand is to create a forecasting model that can reliably estimate sales for a future time frame, leveraging historical sales data and relevant variables. The aim is to enhance business planning and decision-making by providing accurate sales projections for a specified future period."





DESCRIPTION FOR THE DATA SET

Link-https://www.kaggle.com/datasets/chakradharmattapalli/future-sales-prediction
The dataset link mentioned above is related to sales prediction and includes information about different advertising mediums and their impact on sales. Here's what each column likely represents:
1. TV: This column likely represents the advertising budget spent on TV advertising for a specific time period.
2. Radio: This column likely represents the advertising budget spent on radio advertising for the same time period.
3. Newspaper: This column likely represents the advertising budget spent on newspaper advertising.
4. Sales: This column likely represents the actual sales figures for the product or service during the same time period.

With this information, it's understandable that this dataset is used to explore the relationship between advertising expenditures on TV, radio, and newspaper and the resulting sales figures. This type of dataset is often used in marketing and data analysis to build predictive models or understand which advertising channels have the most impact on sales.
To perform a more detailed analysis or build predictive models using this dataset, we are considering tasks such as regression analysis to predict sales based on advertising spending or exploring the correlation between different advertising mediums and sales performance.




CODE EXPLAINATION

This code is a Python script that performs a basic data analysis and linear regression model training on a dataset related to sales. Let's break down the code step by step:

1. First, the necessary libraries are imported: pandas for data manipulation, numpy for numerical operations, matplotlib.pyplot for data visualization, seaborn for enhanced data visualization, and various functions and classes from the sklearn (Scikit-learn) library for machine learning tasks.

2. The dataset is loaded from a CSV file named "sales.csv" using pd.read_csv(), and the DataFrame is stored in the variable df.

3. The script prints the first 5 rows of the dataset using df.head(5).

4. The general information about the dataset is displayed using df.info(). This includes the number of non-null entries in each column and the data types of the columns.

5. The script checks the number of rows and columns in the DataFrame using df.shape and prints the column names using df.columns.

6. It then prints the number of rows and columns in the DataFrame.

7. Data cleaning is performed to check for missing values. The script uses df.isnull().sum() to check for null values in the dataset. If the column 'Unnamed: 0' exists in the DataFrame, it is dropped using df.drop(columns=['Unnamed: 0']).

8. Summary statistics of the dataset are displayed using df.describe(), providing statistics such as count, mean, standard deviation, minimum, and maximum values for each numerical column.

9. The input features (x) are defined as all the columns in the DataFrame except the last one, which is assumed to be the target variable.

10. Exploratory data analysis is performed, including box plots for the 'TV,' 'Newspaper,' and 'Radio' columns and a distribution plot for the 'Newspaper' column.

11. The target variable 'Sales' is defined as y.

12. The script displays the first 2 rows of the DataFrame.

13. It calculates and visualizes the pairwise correlation between each column in the DataFrame using a correlation matrix and a heatmap.

14. The average sales value is computed and printed.

15. A histogram of the 'Sales' column is plotted to show the distribution of sales.

16. Scatter plots are created to visualize the relationship between advertising expenditure ('TV,' 'Radio,' and 'Newspaper') and 'Sales.'

17. The dataset is split into training and testing sets using train_test_split from Scikit-learn.

18. Model training is performed using a Linear Regression model (LinearRegression from Scikit-learn) on the training data. The input and target variables are cast to integers and scaled using StandardScaler.

19. The model is used to make predictions on the test data.

20. Scatter plots are created to visualize the predicted values versus the true values.

21. Model evaluation is performed, calculating metrics like mean squared error (MSE), mean absolute error (MAE), and R-squared.

22. A scatter plot is created to visualize the actual sales versus the predicted sales.

23. A scatter plot and a linear regression line are plotted to visualize the relationship between the input features (xtest) and the target variable (ytest).

In summary, this code loads a sales dataset, performs data cleaning, explores the data through visualizations, splits the data into training and testing sets, trains a linear regression model, evaluates the model's performance, and provides visualizations to help understand the data and model results.





CHALLENGES FACED

We faced challenges while implementing model like linear regression.
MODEL TRAINING PROCESS
 The dataset, which includes advertising expenditures (TV, radio, newspaper) and sales, can be used to build predictive models to understand how advertising spending affects sales. Below are a few modelling approaches you can consider:

1. Linear Regression:
   - Linear regression is a simple yet powerful model for predicting a numerical outcome  based on one or more predictor variables (TV, radio, newspaper).
   - You can build a linear regression model to quantify the relationship between advertising budgets and sales. The coefficients of the model will show the impact of each medium on sales.
2. Multiple Linear Regression:
   - This is an extension of linear regression, which allows you to model the relationship between multiple predictor variables (TV, radio, newspaper) and the target variable (sales).
   - By using multiple linear regression, you can account for the combined effect of all advertising channels on sales.


LIBRARIES NEEDED
Numpy

Pandas

Matplotlib

sklearn

Scipy

Seaborn

pylab



INSTRUCTIONS TO USE
Uploard the dataset for which  sales should be detected use the above mentioned guidelines to do the program and obtain the necessary plot
