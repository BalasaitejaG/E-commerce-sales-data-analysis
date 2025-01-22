# E-commerce Sales Prediction Project

## Business Scenario

This project utilizes historical sales data from 45 Walmart stores across various regions. Each store is composed of multiple departments, and the objective is to forecast sales for each department within each store. The dataset includes details on specific holiday markdown events, which are known to influence sales patterns. Predicting the impact of these markdowns on different departments presents a unique challenge.

## Dataset

Historical sales figures are provided for 45 Walmart stores in diverse locations. The task is to predict sales at the department level for each store.

Walmart implements several promotional markdown events throughout the year, particularly before major holidays such as the Super Bowl, Labor Day, Thanksgiving, and Christmas. Sales during holiday weeks are considered more significant in evaluations. A key aspect of this project is to model the impact of markdowns on sales during these holiday periods, despite potential limitations in historical data.

The core concept of analyzing the Walmart sales data is to understand the factors that influence sales performance in Walmart stores.

## Project Goal

The aim of this project is to develop a predictive model for Walmart sales forecasting, considering various influencing factors.

## Dataset Overview

**stores.csv**

This file contains anonymized details about 45 stores, including store type and size.

**train.csv**

This file provides historical sales data from February 5, 2010, to November 1, 2012. It includes the following fields:

Store - Store identifier
Dept - Department identifier
Date - Week of sales data
Weekly_Sales - Sales for the department in the store for the week
IsHoliday - Indicator for holiday weeks

**test.csv**

This file mirrors the structure of train.csv but excludes the Weekly_Sales data. The task is to predict weekly sales for each store, department, and date combination in this file.

**features.csv**

This file contains supplementary information related to stores, departments, and regional economic indicators for specific dates, including:

Store - Store identifier
Date - Week of data
Temperature - Average regional temperature
Fuel_Price - Regional fuel cost
MarkDown1-5 - Anonymized markdown event data. Markdown data is available from November 2011 onwards and may not be present for all stores or periods. Missing values are denoted as NA.
CPI - Consumer Price Index
Unemployment - Unemployment rate
IsHoliday - Holiday week indicator

For reference, the major holidays within the dataset fall within these weeks:

Super Bowl: Feb 12, 2010; Feb 11, 2011; Feb 10, 2012; Feb 8, 2013
Labor Day: Sep 10, 2010; Sep 9, 2011; Sep 7, 2012; Sep 6, 2013
Thanksgiving: Nov 26, 2010; Nov 25, 2011; Nov 23, 2012; Nov 29, 2013
Christmas: Dec 31, 2010; Dec 30, 2011; Dec 28, 2012; Dec 27, 2013

## Business Objectives and Constraints
* High cost associated with prediction errors.
* Potential need for timely predictions.

## Project Files

1.  **Walmart_Sales_Forecasting.ipynb:** Jupyter notebook containing the sales forecasting model code.
2.  **data/:**  Directory to store the datasets (stores.csv, train.csv, test.csv, features.csv).

## Software Requirements

1.  Jupyter Notebook
2.  Python

## Python Libraries

-   NumPy
-   Pandas
-   Matplotlib and Seaborn
-   Plotly
-   scikit-learn
