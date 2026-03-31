# Bank Marketing Campaign Optimization: Comparing Classification Models

## Overview

This project analyzes a dataset from a Portuguese banking institution related to direct marketing campaigns. The objective is to predict whether a client will subscribe to a term deposit and to compare the performance of multiple classification models.

The analysis focuses on improving campaign efficiency by identifying customers who are more likely to respond positively, allowing for better targeting and more effective use of resources.

---

## Business Problem

Banks run direct marketing campaigns to promote financial products such as term deposits. These campaigns often involve contacting a large number of clients, but the success rate is typically low.

Improving the efficiency of these campaigns requires:

* Identifying clients who are more likely to subscribe
* Reducing the number of unsuccessful contacts
* Allocating resources more effectively

This project aims to build predictive models that support these objectives.

---

## Dataset

The dataset is sourced from the UCI Machine Learning Repository and contains data from multiple direct marketing campaigns conducted by a Portuguese bank.

* Approximately 41,000 observations
* More than 20 features, including:

  * Client attributes (age, job, education, marital status)
  * Financial information (housing loan, personal loan)
  * Campaign-related variables (contact type, previous outcomes)
  * Economic indicators

Target variable:

* `y`: Indicates whether the client subscribed to a term deposit (yes or no)

Note:
The variable `duration` is excluded from modeling because it is only known after a contact is completed and would introduce data leakage.

---

## Methodology

The project follows the CRISP-DM framework:

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modeling
5. Evaluation
6. Recommendations

---

## Models Evaluated

The following classification models are implemented and compared:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Decision Tree
* Support Vector Machine (SVM)

Each model is evaluated using cross-validation and tuned using grid search.

---

## Evaluation Approach

Model performance is assessed using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

Given the class imbalance in the dataset, particular attention is given to recall and ROC-AUC.

---

## Key Findings

* Outcomes from previous campaigns are strong predictors of future success
* Certain client segments show higher likelihood of subscription
* Model performance varies across methods, with some offering a better balance between identifying successful contacts and limiting false positives
* More targeted campaigns can improve efficiency without reducing overall success rates

---

## Recommendations

* Prioritize clients with a higher predicted probability of subscription
* Use previous campaign outcomes to refine targeting strategies
* Reduce the number of low-probability contacts
* Integrate predictive models into campaign planning

---

## Next Steps

* Explore ensemble models such as Random Forest and Gradient Boosting
* Perform feature importance analysis
* Evaluate models using additional business-focused metrics
* Test model performance in a real campaign setting

---

## Repository Structure

## Repository Structure

```text
├── data/
│   └── bank-additional-full.csv
├── Comparing_classification_models.ipynb
└── README.md
---

## References

* Moro, S., Cortez, P., & Rita, P. (2014). A Data-Driven Approach to Predict the Success of Bank Marketing Campaigns
* UCI Machine Learning Repository: Bank Marketing Dataset
