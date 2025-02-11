# Credit Card Fraud Detection Project

## Description
This project analyzes a real-world dataset on credit card fraud detection sourced from Kaggle. The dataset provides insights into fraudulent transactions to help credit card companies identify and prevent fraud.

**Dataset URL:** [Credit Card Fraud Detection | Kaggle]

## Context
Credit card companies aim to recognize fraudulent transactions to ensure customers are not charged for items they did not purchase. This analysis focuses on building models to detect such fraudulent activities.

## Content
The dataset contains transactions made by credit cards in September 2013 by European cardholders. It includes:

- **Total Transactions:** 284,807
- **Fraudulent Transactions:** 492
- **Fraud Percentage:** 0.172% (highly unbalanced dataset)

### Features
- **V1-V28:** Numerical input variables resulting from a Principal Component Analysis (PCA) transformation (original features are confidential).
- **Time:** Seconds elapsed between each transaction and the first transaction in the dataset.
- **Amount:** Transaction amount.
- **Class:** Response variable (labeled outcome), where 1 indicates fraud and 0 indicates a legitimate transaction.

## Conclusion
This project has tested two methods of dimensionality reduction: Univariate Feature Selection (UFS) using the `f_classif` scorer function and Principal Component Analysis (PCA) to reduce the dataset to 10 features. Evaluating primarily by recall and accuracy scores, we found that UFS yielded the best model results during 5-fold cross-validation on the training set.

We then tested three classification algorithms: Logistic Regression, Decision Tree Classifier, and Random Forest Classifier. Using UFS for dimensionality reduction, we trained the models and evaluated their performance on the test set. The Decision Tree Classifier achieved the highest recall score of 0.96, followed closely by Logistic Regression and Random Forest Classifier at 0.94. Regarding accuracy, both the Logistic Regression and Random Forest Classifier scored 0.95, slightly outperforming the Decision Tree Classifier's score of 0.94.

Given the nature of the fraud detection problem, the recall score is paramount; detecting all potential fraud cases is crucial. Therefore, the Decision Tree Classifier demonstrated the best performance in fraud detection for this project.

## Author
Created by Titat Uttawat  
_P.S. This notebook has been adapted from one of the City University of Hong Kong's SDSC2001 coursework._

## Usage
To run the analysis:
1. Clone this repository.
2. Ensure you have the required libraries installed.
3. Load the dataset and follow the analysis steps outlined in the notebook.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
