# LoanDefaultModel

## 1. What is this project?
A crucial function of banks is lending out money to people. To stay in business, they need to predict with reasonable accuracy who will pay back their loans. Figuring out what 
features of a borrower are associated with paying or not paying back a loan has become an increasingly researched topic in the banking industry. In particular, Machine Learning 
techniques are starting to be used to decide whether a person should get a loan. This has led to some debate about the ethics of letting algorithms decide important life outcomes 
and concerns that the models may discriminate against certain groups of people. Although this project will not discuss these issues in detail, it is worth considering these 
questions when implementing them in the real world.

## 2. What does it do?
The code uses data from [Kaggle](https://www.kaggle.com/wordsforthewise/lending-club). The data contains a bunch of features about the loan (e.g. Loan Amount) and the borrower 
(e.g. Employment Length of the borrower). The dependent variable is the column saying whether the loan has been "Fully Paid" or "Charged Off". The Python code 
(`Loan Prediction Modelv3.ipynb`) is in the form of a Jupyter Notebook. The code outputs `loan_prediction_model.h5` which is all the weights and biases it learnt when creating the
model.

## 3. How do I run the code?
The Python code (`Loan Prediction Modelv3.ipynb`) is in the form of a Jupyter Notebook. If you download the code and the data (LoanDefaultModel/Data/) and run it locally; 
it should run and produce the h5 model as an output. 

## 4. What are the results?
The model I created was able to predict with 89% accuracy whether a person would pay back their loan. There were far more people in the dataset who paid back their loans than
those that did not. This means that an 89% accuracy should be considered with caution. In particular, the model classified many people who did default on their loan as "Fully 
Paid". Obviously, no model is perfect and banks are often willing to lend out money where they are not 100% certain that the borrower will pay back the loan.

