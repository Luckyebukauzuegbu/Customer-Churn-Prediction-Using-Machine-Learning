# Customer Churn Prediction Using Machine Learning

## Project Overview

Customer retention is a major challenge for financial institutions, as customer churn can negatively affect revenue growth, customer relationships, and long-term business performance.
This project develops an end-to-end machine learning solution for predicting customers who are likely to churn. The objective is to analyse customer behaviour patterns, build predictive classification models, evaluate model performance, and generate insights that can support proactive customer retention strategies.
The project demonstrates the practical application of machine learning techniques, including data preprocessing, exploratory data analysis, feature engineering, model development, model evaluation, and predictive risk classification.


# Project Objectives

The objectives of this project are to:

- Analyse customer characteristics and behavioural patterns associated with churn.
- Prepare and preprocess customer data for machine learning modelling.
- Develop and compare multiple classification algorithms.
- Evaluate model performance using appropriate classification metrics.
- Identify important factors influencing customer churn risk.
- Develop customer risk categories for retention prioritisation.
- Create a predictive solution that supports data-driven decision-making.

# Dataset Description

The project uses a Nigerian banking customer dataset containing demographic, financial, transactional, engagement, service-experience, and account-behaviour variables.

The dataset was designed for machine learning experimentation and represents a realistic customer churn prediction scenario within a banking environment.

The dataset includes:

- Customer demographic information
- Financial characteristics
- Transaction behaviour
- Account activity indicators
- Customer engagement variables
- Service experience attributes

## Dataset Summary

| Dataset Attribute | Value |
|------------------|------:|
| Customer records | 15,000 |
| Total variables | 48 |
| Model input features | 45 |
| Duplicate records | 0 |
| Missing values | 0 |
| Target variable | Churn_Within_6M |

# Target Distribution

The churn target variable was imbalanced, with more customers classified as non-churners than churners.

| Churn Status | Customers | Percentage |
|-------------|----------:|-----------:|
| No Churn | 12,251 | 81.67% |
| Churn | 2,749 | 18.33% |

Because of the class imbalance, model performance was evaluated beyond accuracy alone using:

- Precision
- Recall
- F1-score
- Balanced accuracy
- Confusion matrix analysis
- ROC-based evaluation


# Machine Learning Workflow

The project followed a complete machine learning workflow:

## 1. Data Preparation

- Data loading and validation
- Data quality checks
- Missing value analysis
- Feature preparation
- Encoding categorical variables

## 2. Exploratory Data Analysis

Exploratory analysis was conducted to:

- Understand customer characteristics
- Identify behavioural patterns linked with churn
- Examine relationships between customer attributes and churn outcomes

## 3. Feature Engineering

Relevant customer features were prepared and transformed to improve model learning and prediction performance.

## 4. Model Development

Multiple classification models were trained and evaluated, including:

- Dummy Classifier
- Logistic Regression
- Random Forest
- Gradient Boosting

## 5. Model Evaluation

Models were assessed using:

- Accuracy
- Precision
- Recall
- F1-score
- Balanced accuracy
- Confusion matrix


# Model Development and Selection

The final selected model was a weighted Gradient Boosting classification pipeline.

The model selection process considered:

- Performance on unseen test data
- Ability to identify actual churn customers
- Balance between false positives and false negatives
- Practical usefulness for customer retention prioritisation

A classification threshold of **0.57** was selected using training data validation before final evaluation.



# Final Model Performance

The final model was evaluated on a held-out test dataset.

| Metric | Result |
|--------|-------:|
| Test customers | 3,000 |
| Accuracy | 79.77% |
| Churn Precision | 45.47% |
| Churn Recall | 52.00% |
| Churn F1-score | 48.52% |
| Balanced Accuracy | 69.00% |
| Customers Flagged | 629 |
| Percentage Flagged | 20.97% |



# Confusion Matrix Summary

| Outcome | Customers |
|---------|----------:|
| True Negatives | 2,107 |
| False Positives | 343 |
| False Negatives | 264 |
| True Positives | 286 |

The model successfully identified 286 out of 550 actual churn customers while maintaining a manageable customer review population.

This demonstrates how machine learning can assist organisations in prioritising customers who may require retention attention.


# Customer Risk Segmentation

The model probability outputs were converted into customer risk categories.

| Risk Level | Probability Range | Observed Churn Rate |
|-----------|------------------:|--------------------:|
| Low Risk | Below 0.30 | 6.18% |
| Moderate Risk | 0.30 - 0.57 | 13.78% |
| High Risk | 0.57 - 0.75 | 33.63% |
| Very High Risk | Above 0.75 | 58.78% |

These risk categories provide a practical way for organizations to prioritise customer retention activities.


# Key Predictive Insights

Feature importance analysis identified several variables associated with higher churn risk, including:

- Customer inactivity patterns
- Active membership status
- Recent transaction decline
- Number of products held
- Account fee characteristics
- Customer engagement behaviour

These findings represent predictive relationships within the dataset and should be validated using real-world customer data before operational deployment.

# Technical Skills Demonstrated

This project demonstrates practical experience in:

- Machine Learning Classification
- Predictive Analytics
- Data Cleaning and Preparation
- Exploratory Data Analysis
- Feature Engineering
- Model Comparison
- Model Evaluation
- Handling Imbalanced Datasets
- Classification Threshold Optimization
- Feature Importance Analysis
- Predictive Risk Modelling


# Tools and Technologies

The project was developed using:

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook
- Streamlit


# Repository Structure

Customer-Churn-Prediction-Using-Machine-Learning

│
├── app/
│   └── Streamlit application files
│
├── data/
│   └── Dataset files and documentation
│
├── notebooks/
│   └── Machine learning analysis notebooks
│
├── outputs/
│   └── Model results and evaluation files
│
├── documentation/
│   └── Supporting project documentation
│
├── requirements.txt
│
└── README.md

# Business Application

Customer churn prediction can help financial institutions and businesses to:

- Identify customers at risk of leaving
- Develop targeted retention strategies
- Improve customer experience
- Support evidence-based decision-making
- Allocate retention resources effectively


# Limitations and Future Improvements

This project represents a machine learning proof of concept and has several limitations:

- The dataset requires validation against real-world customer records before production use.
- Model performance may change when applied to new customer populations.
- Predictions should support human decision-making rather than replace professional judgement.
- Additional feature selection and model optimization could improve efficiency.

Future improvements include:

- Testing on real banking customer datasets
- Developing automated prediction pipelines
- Improving model explainability using advanced interpretation techniques
- Deploying the model as a production-ready application


# Project Status

Completed:

✅ Data preparation and validation  
✅ Exploratory data analysis  
✅ Feature engineering  
✅ Machine learning model development  
✅ Model comparison  
✅ Performance evaluation  
✅ Risk segmentation  
✅ Model validation  

Future Development:

⬜ Production deployment  
⬜ Real-world dataset validation  
⬜ Advanced model explainability  
⬜ Automated ML pipeline integration  


# Conclusion

This project demonstrates the practical application of machine learning for customer churn prediction.

By analyzing customer-behaviour and developing predictive classification models, the solution provides a data-driven approach for identifying customers who may require retention attention.

The project highlights how machine learning can support business decision-making through predictive analytics, customer segmentation, and actionable insights.
