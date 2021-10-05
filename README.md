# ML-for-Fraud-Detection

## Background
Research by the Association of Certified Fraud Examiners (ACFE) found that the “typical organization loses 5% of revenues each year to fraud” with a median loss of $145,000 per case. Traditionally, auditors rely on sampling and manually checking to detect fraud.  Hence, frauds are usually not discovered immediately (the ACFE found the median discovery time was 18 months from the beginning of the fraud).  Recent years, internet companies and banking applied rule-based data analysis for fraud detection.  However, the process of creating rules is time-consuming and involves manual interaction. As the velocity of commerce is increasing, it’s very important to have a quicker solution to detect fraud.

In this project, I try to apply Machine Learning for fraud detection and fraud prevention.  Because ML is good at finding pattern(abnormal pattern in this case) from high volumn of data.  It is scalable to catch the new trend and provide real-time protection to enterprises. 

Sales process is a high risk process in enterprises.  I use lagecy sales dataset from a Global 500 manufacturer for fraud detection.  

### Project steps
1. Data cleaning and Feature selection.
  * Main source data was exported from SAP, csv format with  200k+ records, 93 fields. 
  * Import csv into Pandas Dataframe.
  * Studied and selected useful feature.  Final confirmed 19 fields from 93 fields.
  * Filled missing value with appropriate value.  
2. Exploratory analysis to understand data.
![Sales by date](p1.npg) 
4. Feature selection and feature engineering. 
5. Model selection and training. 
6. Model evaluation. 
