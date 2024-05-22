
## Table of Contents.
- [Title and Description](#SYRIATEL-Customer-Churn.)
- [Business Understanding](#Business-Understanding.)
- [Data Understanding](#Data-Understanding.)
- [Project Structure](#Project-Structure.)
- [Installation.](#Installation.)
- [How To Use](#How-To-Use.)
- [Data Preprocessing](#Data-Preprocessing.)
- [Model Training](#Model-Training.)
- [Model Evaluation](#Model-Evaluation.)
- [Feature Importance](#Feature-Importance.)
- [Results](#Results.)
- [Conclusion](#Conclusion.)
- [Recommendations](#Recommendations.)
- [References.](#References.)
- [Author.](#Author.)
# SYRIATEL Customer Churn.

This project aims to predict customer churn using various machine learning models. The dataset used for this project contains customer details and their subscription information.


## Business Understanding.
- ***Business Problem:***
  Predict whether a customer will stop doing business with SyriaTel, a telecommunications company.
 - ***Stakeholder:***
  SyriaTel(Customer Retention Department)
 - ***Stakeholder objective:*** 
  Reduce customer churn by understanding key predictors and implementing targeted retention strategies.

## Data Understanding.
The dataset includes features such as area code, international plan, voice mail plan, total minutes (domestic and international), number of customer service calls, and total charges.

## Project Structure.
1. project_phase3.ipynb: Jupyter notebook with the entire workflow
2. SyriaTel_Churn.ppt: Non-technical presentation.
3. README.md: Project documentation
## Installation.
To run this project, you'll need the following libraries:
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

Install the required libraries using:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```


##  How To Use.
1. Clone the repository
2. Install the required libraries
3. Run the project_phase3.ipynb notebook.
Open the notebook in your preferred Jupyter environment and execute the cells.

## Data Preprocessing.
- One-hot encoded categorical features
- Normalized numerical features
- Dropped unneccesary columns.

## Model Training.
We trained three models:

1. Logistic Regression
2. Random Forest
3. Gradient Boosting
Hyperparameter tuning was performed using GridSearchCV.
## Model Evaluation.
The models were evaluated using the following metrics:

- ROC-AUC
- F1 Score
- Precision
- Recall
- Accuracy
## Feature Importance.
- **Total Charge** was the most crucial feature in both models(Random Forest, Gradient Boosting).
- **Customer Service Calls** was consistently important.
- **International Features** like total international minutes and having an international plan also played significant roles.
- **Area Codes** had minimal impact on predicting churn.

## Results.
**Logistic Regression:**
- ROC-AUC: 0.845
- F1 Score: 0.415
- Precision: 0.659
- Recall: 0.303
- Accuracy: 0.772
**Random Forest:**
- ROC-AUC: 0.932
- F1 Score: 0.934
- Precision: 1.000
- Recall: 0.876
- Accuracy: 0.981
**Gradient Boosting:**
- ROC-AUC: 0.933
- F1 Score: 0.929
- Precision: 0.987
- Recall: 0.876
- Accuracy: 0.978
## Conclusion.
- Random Forest and Gradient Boosting models performed exceptionally well.
- Logistic Regression showed lower performance, indicating it might not be the best choice for this dataset.
## Recommendations.
- Observe competitor international plans and adjust your charges and service delivery in turn.
- Observe the conduct in the customer service call centre, and make any changes to the personell and/or the code of conduct. Make sure to log the different complaints/issues recorded in the call and make sure they are addressed immediately.
- Encourage the promotion of voicemail plans as people with voicemail plans are less likely to churn.

## References.
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Matplotlib Documentation](https://matplotlib.org/stable/index.html)
## Author.
- [@LeonMaina](https://www.github.com/maina-leon)# Syriatel_Churn
