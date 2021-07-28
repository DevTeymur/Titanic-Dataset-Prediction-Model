##Titanic dataset model prediction

#Variable Notes
pclass: A proxy for socio-economic status (SES)
1st = Upper
2nd = Middle
3rd = Lower

age: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5

sibsp: The dataset defines family relations in this way...
Sibling = brother, sister, stepbrother, stepsister
Spouse = husband, wife (mistresses and fiancés were ignored)

parch: The dataset defines family relations in this way...
Parent = mother, father
Child = daughter, son, stepdaughter, stepson
Some children travelled only with a nanny, therefore parch=0 for them.

#Needed python libraries:
Pandas, matplotlib, seaborn, filterwarnings, numpy, sklearn, xgboost

#General Process
Some graphs displayed with different parameters to have idea about dataset.
All outliers and missing values were handled.
Labels encoded and with the help of GridSearchCV best parameters gotten from each model.
Best model was Logistic Regression with 88.14% model accuracy with solver='liblinear', multi_class='auto', C=47 values.