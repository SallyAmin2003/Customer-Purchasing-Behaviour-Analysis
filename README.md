# Customer Purchasing Behaviour and Market Basket Analysis Using PySpark

## Overview

This project analyses the Online Retail II dataset using PySpark to discover customer purchasing patterns, identify frequently purchased product combinations, classify invoice value, and detect unusual transactions.

The project demonstrates large-scale data mining techniques including market basket analysis, machine learning classification, dimensionality reduction, and anomaly detection.

## Dataset

Online Retail II Dataset (UCI Machine Learning Repository)

- More than 1 million transaction records
- UK-based online retailer
- Transaction data from 2009–2011
- Invoice, customer, product, quantity, country, and price information

## Technologies Used

- Python
- PySpark
- Spark SQL
- Spark MLlib
- Google Colab
- Pandas

## Data Processing

- Removed missing customer IDs and product descriptions
- Removed cancelled invoices
- Removed negative quantities and prices
- Created Revenue feature
- Saved cleaned dataset as Parquet format

Final cleaned dataset:

- 805,549 transactions

## Exploratory Data Analysis

Investigated:

- Top countries by revenue
- Product sales trends
- Revenue distribution
- Customer purchasing patterns

Key finding:

- The United Kingdom generated approximately £14.72 million in revenue and dominated transaction volume.

## Market Basket Analysis

Implemented FP-Growth for association rule mining.

Generated:

- Frequent itemsets
- Association rules
- Product recommendations

Example findings:

- Product families such as POPPY'S PLAYHOUSE items showed strong purchasing relationships.
- Several matching tea cup and saucer products produced high-confidence rules.

Applications:

- Product recommendations
- Cross-selling
- Promotional bundles
- Website product placement

## Machine Learning Models

### Naive Bayes

Used for high-value invoice prediction.

Results:

- Accuracy: 0.631
- Weighted F1 Score: 0.631

### Linear Support Vector Machine (SVM)

Used for high-value invoice prediction.

Results:

- Accuracy: 0.818
- Weighted F1 Score: 0.818

The SVM model significantly outperformed Naive Bayes.

## PCA Analysis

Applied Principal Component Analysis (PCA) to understand feature variance.

Results:

- PC1 explained 55.86% of variance
- PC2 explained 44.14% of variance

## Anomaly Detection

Implemented IQR-based anomaly detection.

Results:

- 3,020 unusual invoices identified
- Largest anomaly generated revenue of £168,469.60

Applications:

- Fraud detection
- Business auditing
- Wholesale order monitoring

## Skills Demonstrated

- Big Data Analytics
- Data Mining
- Market Basket Analysis
- FP-Growth
- Machine Learning
- SVM Classification
- Naive Bayes Classification
- PCA
- Anomaly Detection
- PySpark
- Data Cleaning
- Feature Engineering

## Future Improvements

- Isolation Forest anomaly detection
- Recommendation systems
- Customer segmentation
- Advanced fraud detection
- Deep learning approaches
