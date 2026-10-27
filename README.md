
# Predicting On-Time Delivery in a Supply Chain Using Weka

A machine learning classification project that predicts whether a shipment will reach its destination on time or be delayed, using historical logistics data and the Weka machine learning toolkit.

## Overview

Delivery delays can affect customer satisfaction, logistics costs, and supply chain efficiency. This project explores how machine learning classification algorithms can be used to analyze shipment data and predict delivery timeliness.

Using Weka, three classification algorithms were evaluated and compared to identify the best-performing model for the dataset.

## Objectives

- Analyze historical shipment data.
- Build classification models to predict delivery timeliness.
- Compare the performance of different machine learning algorithms.
- Evaluate models using accuracy, Cohen's Kappa statistic, and classification metrics.
- Examine ROC curves and classifier evaluation outputs.

## Dataset

The dataset contains **10,999 records and 12 attributes** describing shipments and their associated characteristics.

The attributes cover information such as:

- Warehouse block
- Mode of shipment
- Customer calls
- Customer rating
- Product cost
- Prior purchases
- Product importance
- Gender
- Discount offered
- Product weight
- Delivery status

**Target variable:** `Reached.on.Time_Y.N`

This attribute represents the delivery outcome used for classification.

## Machine Learning Algorithms

Three algorithms were evaluated using Weka:

| Algorithm | Accuracy | Cohen's Kappa |
|---|---:|---:|
| Naive Bayes | 68.52% | 0.41 |
| Random Forest | 65.89% | 0.32 |
| Logistic Regression | 65.59% | 0.29 |

*Results are transcribed from the project report.*

## Results and Analysis

### 1. Naive Bayes

Naive Bayes achieved the highest reported accuracy of **68.52%**, with a Kappa statistic of 0.41. It performed best among the three evaluated algorithms.

### 2. Random Forest

Random Forest achieved **65.89% accuracy** and a Kappa statistic of 0.32. The model provides a tree-based classification approach for analyzing shipment characteristics.

### 3. Logistic Regression

Logistic Regression achieved **65.59% accuracy** and a Kappa statistic of 0.29. Its performance was comparable to Random Forest on this dataset.

### Key Finding

Naive Bayes was the best-performing model among the three algorithms evaluated in this experiment. The results indicate potential for further improvement through feature engineering, hyperparameter tuning, and additional model evaluation.

## Tools and Technologies

- **Weka** — Machine learning experimentation and classification
- **Machine Learning** — Supervised classification
- **Data Analysis** — Shipment attribute analysis
- **Model Evaluation** — Accuracy, Cohen's Kappa, ROC curves, and classification metrics

## Methodology

1. Load the shipment dataset into Weka.
2. Inspect the dataset attributes and distributions.
3. Set the delivery outcome as the target class.
4. Evaluate Random Forest, Naive Bayes, and Logistic Regression.
5. Use 10-fold cross-validation, as documented in the report.
6. Compare model evaluation results.
7. Identify the best-performing algorithm.

## Repository Contents

- `Weka_Project_Report_Template_Jahnavi_S_SrinagG.docx` — Project report containing the methodology, Weka screenshots, evaluation results, and conclusion.

## Limitations and Future Improvements

The reported model accuracy is moderate, leaving room for improvement. Potential next steps include:

- Tuning Random Forest parameters, including the number of trees and tree depth.
- Improving feature selection and engineering.
- Comparing additional classification algorithms.
- Evaluating precision, recall, F1-score, and confusion matrices for each class.
- Investigating class imbalance and the causes of delivery delays.
- Developing a reproducible workflow for retraining and evaluating the models.

## Conclusion

This project demonstrates the application of supervised machine learning to a supply chain delivery prediction problem using Weka. Three classification algorithms were evaluated, with Naive Bayes achieving the highest reported accuracy of 68.52%.

The experiment provides a foundation for exploring how predictive analytics can support logistics planning and delivery performance analysis.

## Author

**Jahnavi S Srinag**

Machine Learning | Artificial Intelligence | Data Analytics

---

*Note: The results presented here reflect the experiments documented in the project report. The repository currently contains the report; the original dataset and runnable experiment files are not included.*
