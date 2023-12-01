# project_3

# SyriaTel Customer Churn Prediction


![alejandro-barba-Oq0paHvp1gg-unsplash](https://github.com/RuthNanjala/project_3/assets/141912190/c798e954-d6a1-4ee1-897d-d2cad7e884c3)


## Overview
In the dynamic landscape of the telecommunications industry, customer retention plays a pivotal role in sustaining business success. This data science project is centered around predicting customer churn for SyriaTel, a leading telecommunications company. The primary goal is to develop a robust classification model capable of forecasting whether a customer is likely to terminate their association with SyriaTel. This predictive capability empowers businesses to proactively address customer retention challenges, minimizing financial losses and enhancing strategic decision-making.

## Introduction
Given the fiercely competitive nature of the telecommunications industry, customer retention is crucial for sustaining a thriving business. Recognizing the significance of predicting customer churn, we aim to leverage advanced data science techniques to provide SyriaTel with actionable insights. Through the analysis of a carefully chosen dataset and the application of classification models, we seek to empower SyriaTel to anticipate customer behavior and implement targeted strategies for customer retention.

## Challenges
The dataset comprises intricate features that necessitate meticulous consideration and engineering to derive meaningful insights. The presence of imbalanced classes, with churn instances being a minority, introduces challenges related to potential bias in model predictions. Given the dynamic nature of customer behavior, capturing temporal patterns becomes imperative for ensuring accurate predictions. Striking a balance between model interpretability and complexity poses a challenge, especially when selecting the most suitable algorithm for the task.

## Proposed Solution
The proposed solution involves a meticulous process of data exploration, analysis, and modeling. The intricate features within the dataset demand careful consideration and engineering to derive meaningful insights. Imbalanced classes, with churn instances being a minority, necessitate strategies to mitigate potential bias in model predictions. The dynamic nature of customer behavior requires specific attention to ensure accurate predictions. Balancing the trade-off between model interpretability and complexity is another crucial aspect, guiding our careful selection of algorithms that align with the dataset's intricacies.

## Brief Conclusion
The mission is clear, to provide SyriaTel with a predictive tool that enhances their strategic decision-making. The subsequent sections will delve into the project intricacies, from dataset understanding to the technical nuances of model selection and evaluation.

## Problem Statement
In the fiercely competitive landscape of the telecommunications industry, maintaining customer loyalty is pivotal for sustained business prosperity. SyriaTel, a prominent entity in this dynamic sector, confronts the intricate task of foreseeing and curtailing customer churn. Navigating the intricacies of customer interactions amid the ever-evolving industry demands a proactive, data-driven strategy to effectively tackle the challenges associated with churn.

## Objectives
1.Identify and interpret key features influencing customer churn.
2.Explore Relationships Between Key Features Influencing Customer Churn.
3.Develop a classification model with high accuracy to predict customer churn for SyriaTel.

## Business and Data Understanding

### Stakeholder Audience
The primary stakeholders for this project include:
SyriaTel Executives and Decision-Makers: This analysis aims to provide actionable insights for strategic decision-making related to customer retention. Executives can leverage the predictive model to implement targeted strategies, ultimately reducing churn and optimizing customer satisfaction.
Marketing and Customer Service Teams: Insights derived from the analysis can guide marketing efforts and customer service initiatives. Understanding the key factors influencing churn enables these teams to design campaigns and services that resonate with customer needs.
Data Science and Analytics Teams: For technical teams within SyriaTel, this project serves as a demonstration of advanced data science techniques in a real-world scenario. The methodology and results provide a foundation for further exploration and model refinement.
Dataset Choice
The dataset used in this project is the SyriaTel Customer Churn dataset, sourced from Kaggle. It comprises 21 columns and 3333 entries, offering a comprehensive view of customer interactions with SyriaTel. Key features include customer demographics, subscription status to specific services, call durations during different times of the day, and customer service-related metrics.

## Modeling
### Challenges
The dataset poses several challenges that influence the modeling approach:
Imbalanced Classes: The presence of imbalanced classes, with churn instances being a minority, requires strategies to mitigate potential bias in model predictions.
Temporal Patterns: Given the dynamic nature of customer behavior, capturing temporal patterns becomes imperative for ensuring accurate predictions.
Model Complexity: Striking a balance between model interpretability and complexity is crucial. The selection of the most suitable algorithm needs to align with the dataset's intricacies.

## Methodology
The modeling process involves the following steps:
Data Exploration and Analysis: Meticulous exploration of the dataset, including initial data analysis, distribution of churn labels, and identification of key features influencing customer churn.
Data Preprocessing: Handling missing values, encoding categorical variables, and splitting the dataset into training and testing sets.
Baseline Model: Training a baseline logistic regression model to establish a performance baseline.
Random Forest Model: Building a Random Forest model, an ensemble learning method, to improve predictive accuracy.
Hyperparameter Tuning: Fine-tuning the Random Forest model's hyperparameters to optimize performance.
Evaluation: Assessing model performance using metrics such as accuracy, precision, recall, F1-score, and the area under the ROC curve (AUC-ROC).

### Evaluation
Baseline Model: Logistic Regression
Results:
Accuracy: 84.56%
Classification Report:
Precision (Churn): 33%
Recall (Churn): 2%
F1-Score (Churn): 4%
Confusion Matrix:
True Negatives (Non-churn): 562
False Positives (Churn): 4
False Negatives (Non-churn): 99
True Positives (Churn): 2

 ![BL WS](https://github.com/RuthNanjala/project_3/assets/141912190/fb6fc3ad-1fec-4339-b4bd-2c9ce2f21d72)

Interpretation:
The baseline logistic regression model achieved an accuracy of 84.56% but demonstrated low recall for the churn class, indicating its limitations in identifying instances of churn.

SMOTE Model: Logistic Regression
Results:
Accuracy: 68.82%
Classification Report:
Precision (Churn): 27%
Recall (Churn): 63%
F1-Score (Churn): 38%
Confusion Matrix:
True Negatives (Non-churn): 395
False Positives (Churn): 171
False Negatives (Non-churn): 37
True Positives (Churn): 64

 ![BL WWS](https://github.com/RuthNanjala/project_3/assets/141912190/7834c330-21ea-4925-adad-ecc66e8ed4db)

Interpretation:
The logistic regression model with SMOTE-resampled data achieved higher recall for the churn class, indicating better identification of instances of churn, albeit with a decrease in overall accuracy.

Random Forest Model (Untuned)
Results:
Accuracy: 94.82%
Classification Report:
Precision (Churn): 96%
Recall (Churn): 93%
F1-Score (Churn): 95%
Confusion Matrix:
True Negatives (Non-churn): 565
False Positives (Churn): 20
False Negatives (Non-churn): 39
True Positives (Churn): 516
ROC-AUC Score: 98.95% 

![URFM](https://github.com/RuthNanjala/project_3/assets/141912190/d2b4d62c-bc98-4c92-a928-170ff5066300)

Interpretation:
The random forest model demonstrated high accuracy and balanced precision and recall for the churn class, indicating good overall predictive performance.

Random Forest Model (Tuned)
Results:
Accuracy: 95.26%
Classification Report:
Precision (Churn): 97%
Recall (Churn): 94%
F1-Score (Churn): 95%
Confusion Matrix:
True Negatives (Non-churn): 567
False Positives (Churn): 18
False Negatives (Non-churn): 36
True Positives (Churn): 519
ROC-AUC Score: 99.07%

![TRFM](https://github.com/RuthNanjala/project_3/assets/141912190/765b6caf-ffd8-44df-9a12-fd37c76b6bb3)

Interpretation:
The tuned random forest model outperformed the untuned model, achieving higher accuracy and an impressive ROC-AUC score of 99.07%, indicating superior discrimination between positive and negative classes.
In conclusion:
The logistic regression baseline model, while providing an initial benchmark, showed limitations in identifying instances of churn.
The SMOTE logistic regression model, designed to address class imbalance, improved recall for the churn class but resulted in reduced overall accuracy.
The random forest model, especially after hyperparameter tuning, exhibited robust predictive performance, achieving high accuracy, precision, and recall. The tuned model's superior ROC-AUC score indicates its effectiveness in distinguishing between churn and non-churn instances.
The tuned random forest model stands out as the preferred choice for predicting customer churn for SyriaTel, offering a balance between accuracy and effective identification of churn instances. Further deployment and monitoring of this model are recommended for real-time churn prediction.

## Recommendations
Based on the findings, the following recommendations are made:
Implement Targeted Marketing Campaigns: Leverage insights into key features influencing churn to design targeted marketing campaigns. Addressing customer pain points identified in the analysis can enhance the effectiveness of these campaigns.
Enhance Customer Service Initiatives: Focus on improving customer service experiences, especially for segments identified as having a higher likelihood of churn. Proactive measures, such as personalized support, can significantly impact customer satisfaction.
Continuous Monitoring and Model Refinement: Establish a system for continuous monitoring of customer churn patterns. Periodically update the model with fresh data and refine it to adapt to evolving customer behaviors.

## Future Improvements
To further enhance the model and its applications, we should consider the following future improvements:
Feature Engineering: Explore additional features or derive new variables that might contribute to better predictive performance.
Ensemble Models: Experiment with ensemble models combining different algorithms to harness the strengths of each, potentially improving overall model accuracy.
Customer Feedback Integration: Integrate direct customer feedback into the model training process to capture subjective aspects influencing churn.1

## Next Steps
Deploy the tuned Random Forest model into a production environment, integrating it into SyriaTel's operational systems for real-time predictions.
Establish a feedback loop for continuous improvement, incorporating insights from the model predictions into business strategies and assessing the impact on customer retention.
Encourage collaboration between data science, marketing, and customer service teams to ensure a holistic approach to customer retention, aligning strategies with the model's insights.
Conduct educational initiatives to familiarize relevant stakeholders with the model's capabilities and limitations, fostering a data-driven culture within SyriaTel.






