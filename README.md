# Diabetes-Prediction
Ankita Priya

*Pre-final year CS undergrad @[B.I.T Mesra](bitmesra.ac.in)*

## Purpose of Repository
Analysing the Pima Indians Diabetes Dataset for research purpose. 

## Coding Language, IDE and  Libraries used 
All coding woeks are done in Python 3.8 and the IDE used to create them was using Anaconda's **Jupyter Notebook**, you can download Anaconda [here](https://www.anaconda.com/products/individual). 

The Machine Learning models are coded using the following libraries:
- Scikit-learn
- NumPy
- Matplotlib 
- Pandas
- Seaborn


## About the Dataset 
The Pima Indian Diabetes Dataset has been used in this study, provided by the UCI Machine Learning Repository. The dataset has been originally collected from the National Institute of Diabetes and Digestive and Kidney Diseases. The dataset consists of some medical distinct variables, such as pregnancy record, glucose concentration, diastolic blood pressure, BMI, insulin level, age, triceps skin fold thickness, diabetes pedigree function i.e. **nine features** in total. This dataset has 768 patient’s data where all the patients are female and at least 21 years old of [Pima Indian](https://en.wikipedia.org/wiki/Pima_people) heritage. 

Dataset used: https://www.kaggle.com/uciml/pima-indians-diabetes-database

### Data Cleaning
I had to perform data cleaning here because the data has many missing values. The values are not in the form of NaN rather, they are presented as values 'zero'. I replaced all those values by two methods:
1. Taking mean of all the values given and replacing all the zeroes. 
2. Taking median of all the values and replacing all the zero values. 

Data was replaced in the following features:
1. Glucose level: The level cannot be above 150mg/dl or below 70mg/dl. A glucose level of 200 mg/dl or higher is used to diagnose diabetes.
2. Blood Pressure: Diastolic Blood Pressure below 55 and higher than 90 is highly dangerous. 
3. Skin Thickness: This value depicts the body fat. The avg. value is 23 mm in women. 
4. BMI index: Body Mass Index is usually 18.5 to 25. BMI between 25 and 30 falls in the overweight range. A BMI of 30 or over falls in the obese range.

### Algorithms Used 

The Machine Learning algorithms used are:
- Logistic Regression
- K-Nearest Neighbor(KNN)
- Support Vector Classifier -> A class of SVM 
- Random Forest Classification

### Use of this model
This model is used for a research on feature selection and its behaviours with different algorithms. 

Best value was obtained from *Logistic Regression Algorithm* on 5 features namely, Pregnancies, Glucose, Blood Pressure, Skin Thickness and Age without any manipulation with the data. The accuracy obtained was `81.0%`. 
The precision and recall obtained were `80.0%` and `65.0%` respectively. 

## References 
```
Dataset: https://www.kaggle.com/uciml/pima-indians-diabetes-database

Reference site: https://towardsdatascience.com/end-to-end-data-science-example-predicting-diabetes-with-logistic-regression-db9bc88b4d16
```
