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
  * Sales by date
![](https://github.com/ryanhao1115/ML-for-Fraud-Detection/blob/main/p1.PNG) 
  * Sales by branch
![](https://github.com/ryanhao1115/ML-for-Fraud-Detection/blob/main/p2.PNG)
  * Branch - Procls heatmap
![](https://github.com/ryanhao1115/ML-for-Fraud-Detection/blob/main/p3.PNG)
  * Sale amount distribution
![](https://github.com/ryanhao1115/ML-for-Fraud-Detection/blob/main/p4.PNG)
3. Active Learning.
  * There are only 11 invoice, 154 records labeled as fraud transactions.  Others are unlabel data.
  * Created and trained a Neural Network.
  * Predict on unlabel data, selected top 200 uncertain records for review. 
  * Got back 200 records labeled data.  
4. Feature engineering.
  * There were couple categorical fields with too many classes. 
  * Tried Ordinal Encoding
  * Tried One hot encoding, after ignore those fields.
5. The target class - fraud is huge imbalance.
  * Under sampling
  * SMOTE over sampling
6. Created and built a Neural Network for predicting fraud. 
7. Created and built RandomForest Model for predicting fraud.
8. Evaluated and compared results.  
