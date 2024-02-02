# Credit-card-default-classification-model

## Motivation:

As the number of credit card users continues to rise, financial institutions are grappling with an increasing rate of credit card defaults. This surge in defaults not only results in losses for both the banks and the cardholders but also underscores the need for effective solutions. Data analytics emerges as a key tool to address this phenomenon and manage credit defaults. This project explores the implementation of a model that predicts the likelihood of a given credit card holder defaulting in the following month, leveraging their demographic and behavioral data from the preceding 6 months.

## About the Dataset:

The study utilizes the "Default of credit card clients" dataset from the UCI machine learning repository, accessible at the provided link. Comprising 30,000 observations representing distinct credit card clients, each observation encompasses 24 attributes. These attributes encompass details on default payments, demographic factors, credit data, payment history, and credit card statements of clients in Taiwan from April 2005 to September 2005.

The initial set of variables focuses on the client's personal information:

ID: Categorical variable representing the client's ID
LIMIT_BAL: Amount of credit in NT dollars, covering individual and family/supplementary credit
SEX: Gender (1=male, 2=female)
EDUCATION: Level of education (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)
MARRIAGE: Marital status (1=married, 2=single, 3=others)
AGE: Age in years
The subsequent attributes provide information about past payment delays for specific months:

PAY_0 to PAY_6: Repayment status from September 2005 to April 2005 (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months, … 8=payment delay for eight months, 9=payment delay for nine months and above)
Other variables pertain to the amount of bill statements issued monthly by credit card companies:

BILL_AMT1 to BILL_AMT6: Amount of bill statement from September 2005 to April 2005 in NT dollars
The following variables focus on the amount of previous payments made in specific months:

PAY_AMT1 to PAY_AMT6: Amount of previous payment from September 2005 to April 2005 in NT dollars

The final variable for prediction is:

default.payment.next.month: Indicates whether the credit card holders are defaulters or non-defaulters (1=yes, 0=no)
The primary objective is to distinguish clients predicted to default on their credit cards in the next month, based on the "default.payment.next.month" column, where "0" denotes non-defaulters and "1" denotes defaulters.

## Classification algorithms used:

1) Logistic regression
2) Naive Bayes
3) Perceptron 
