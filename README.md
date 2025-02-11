# Credit-Card-Fraud-Detection-Project

## Description
This project analyzes a real-world dataset on credit card fraud detection sourced from Kaggle. The dataset provides insights into fraudulent transactions to help credit card companies identify and prevent fraud.

**Dataset URL:** [Credit Card Fraud Detection | Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

## Context
Credit card companies aim to recognize fraudulent transactions to ensure that customers are not charged for items they did not purchase. This analysis focuses on building models to detect such fraudulent activities.

## Content
The dataset contains transactions made by credit cards in September 2013 by European cardholders. It includes:

- **Total Transactions:** 284,807
- **Fraudulent Transactions:** 492
- **Fraud Percentage:** 0.172% (highly unbalanced dataset)

### Features
- **V1-V28:** Numerical input variables resulting from a Principal Component Analysis (PCA) transformation (original features are confidential).
- **Time:** Seconds elapsed between each transaction and the first transaction in the dataset.
- **Amount:** Transaction amount.
- **Class:** Response variable (labelled outcome), where 1 indicates fraud and 0 indicates a legitimate transaction.

## Author
Created by Titat Uttawat  
_P.S. This notebook has been adapted from one of the City University of Hong Kong's SDSC2001 coursework._

## Usage
To run the analysis:
1. Clone this repository.
2. Ensure you have the required libraries installed.
3. Load the dataset and follow the analysis steps as outlined in the notebook.
