# Store Sales Business EDA

## About the Project

In this project, I performed Exploratory Data Analysis (EDA) on store sales and business data using Python.

The main purpose of this project was to understand store performance by analyzing sales, customers, operating cost, profit, basket size, store type, location and other business-related factors.

I used Python libraries such as Pandas, NumPy, Matplotlib and Seaborn for data analysis and visualization.

## Dataset

The dataset contains **32 rows and 15 columns** related to different stores.

Some important columns used in the analysis are:

* StoreCode
* StoreName
* StoreType
* Location
* OperatingCost
* Staff_Cnt
* TotalSales
* Total_Customers
* AcqCostPercust
* BasketSize
* ProfitPercust
* OwnStore
* OnlinePresence
* Tenure
* StoreSegment

## What I Did in This Project

### 1. Data Loading

* Loaded the store dataset using Pandas.
* Checked the first and last few records.
* Checked the shape and column names.

### 2. Data Cleaning

* Checked missing values.
* Found missing values in `AcqCostPercust`.
* Filled the missing values using the mean.
* Checked duplicate records.
* Checked data types.
* Converted suitable categorical columns into category datatype.

### 3. Data Standardization

I also corrected some inconsistent categorical values:

* `Electronincs` → `Electronics`
* `Banglore` → `Bangalore`

This helped keep the categorical data more consistent for analysis.

### 4. Descriptive Analysis

I used statistical methods to understand the data, including:

* Mean
* Median
* Mode
* Minimum
* Maximum
* Standard deviation
* Quartiles

I also used `describe()` to get an overall statistical summary of the numerical columns.

### 5. Business Analysis

I compared different business metrics using GroupBy operations.

Some of the analysis included:

* Average sales by store type
* Average sales by location
* Average profit by store type
* Average customers by store type
* Average operating cost by store type
* Average basket size by store type
* Average tenure by store type
* Average sales by store segment
* Average sales based on own-store status
* Average sales based on online presence
* Store type and location-wise sales comparison

### 6. Correlation Analysis

I used NumPy to check relationships between important business variables.

For example:

* Total Customers vs Total Sales
* Operating Cost vs Total Sales
* Acquisition Cost per Customer vs Profit
* Basket Size vs Total Sales
* Tenure vs Total Sales

One of the stronger relationships found in the analysis was between **Basket Size and Total Sales**, with a positive correlation of approximately **0.89**.

### 7. Data Visualization

I created visualizations to understand the data more clearly.

The analysis includes plots such as:

* Scatter plots
* Box plot for outlier checking
* Business comparison charts

The visualizations helped me understand relationships between operating cost, sales and other business metrics.

## Key Observations

From my analysis:

* Electronics stores had the highest average sales among the three store types.
* Mumbai had the highest average total sales among the locations analyzed.
* Total customers showed a strong positive relationship with total sales.
* Basket size also showed a strong positive relationship with total sales.
* Operating cost showed a strong negative relationship with total sales in this dataset.
* Different store segments showed noticeable differences in average sales and profit.

These observations are based on the dataset used in this project.

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Project Structure

```text
Store-Sales-Business-EDA/
│
├── Store_Sales_Business_EDA.ipynb
└── README.md
```

## What I Learned

Through this project, I practiced:

* Data cleaning with Pandas
* Handling missing values
* Checking duplicates
* Working with categorical data
* Descriptive statistics
* GroupBy and aggregation
* Correlation analysis
* Data visualization
* Extracting business insights from data

## Conclusion

This project helped me practice the complete basic EDA workflow, starting from loading and cleaning the data to analyzing business metrics and creating visualizations.

It also helped me understand how Python can be used to convert raw business data into useful insights.
