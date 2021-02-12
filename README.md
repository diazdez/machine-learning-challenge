# machine-learning-challenge


# Machine Learning Homework - Exoplanet Exploration

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.
To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

**In this homework assignment, you will need to:**

- [Preprocess the raw data](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)
- Tune the models
- Compare two or more models

## Instructions 

**Preprocess the Data**

- Preprocess the dataset prior to fitting the model.
- Perform feature selection and remove unnecessary features.
- Use MinMaxScaler to scale the numerical data.
- Separate the data into training and testing data.


**Tune Model Parameters**

- Use GridSearch to tune model parameters.
- Tune and compare at least two different classifiers.


**Reporting**

- Create a README that reports a comparison of each model's performance as well as a summary about your findings and any assumptions you can make based on your model (is your model good enough to predict new exoplanets? Why or why not? What would make your model be better at predicting new exoplanets?).


**Hints and Considerations**
- Start by cleaning the data, removing unnecessary columns, and scaling the data.
- Not all variables are significant be sure to remove any insignificant variables.
- Make sure your sklearn package is up to date.
- Try a simple model first, and then tune the model using GridSearch.
- When hyper-parameter tuning, some models have parameters that depend on each other, and certain combinations will not create a valid model. Be sure to read through any warning messages and check the documentation

**Submission**
- Create a Jupyter Notebook for each model and host the notebooks on GitHub.
- Create a file for your best model and push to GitHub
- Include a README.md file that summarizes your assumptions and findings.
- Submit the link to your GitHub project to Bootcamp Spot.
- Ensure your repository has regular commits (i.e. 20+ commits) and a thorough README.md file

====================================================================

# Analysis:

## Model1 and Model1a: Logistic Regression

**Model1:** After cleaning the data I used all the columns, which resulted in a good scores:
-	Training Data Score: 0.9945105215004575
-	Testing Data Score: 0.9935956084172004

**Model1a:** The X values varied because only a “selected” number of columns were selected, which resulted in different scores. So this help confirm that the data from specific columns impacted the score results. For example X values for “selected3_features” returned the following: 

-	Training Score: 0.8854833790789874
-	Testing Score: 0.8815187557182068

## Model2: SVM

**Model2:** similar to Model1, used all the columns for the X values (with the exception of y value column), the scores resulted the same. I
-	Training Score: 0.9945105215004575
-	Testing Score: 0.9935956084172004

There did not appear to be a difference with using Logistic Regression and SVM. 




