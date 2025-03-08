# H1n1_Classification
## Business Goal
### Understanding H1N1 Virus infection:
Identify key factors that influence one contracting h1n1 virus.

### Identifying Trends:
Explore patterns across various categorical variables and their influence in contracting h1n1 virus
### Recommendations
	Provide actionable recommendations to on whether given various features, we can be able to classify whether someone had h1n1 or the seasonal flu.

## Data understanding
As the world struggles to vaccinate the global population against COVID-19, an understanding of how people’s backgrounds, opinions, gender, race, age, health behaviors and other features are related to their personal vaccination patterns can provide guidance for future public health efforts. We try to understand better based on data collected to guide public health efforts in predicting whether one has a likelihood of contracting H1N! virus.

More info can be found here > https://www.drivendata.org/competitions/66/flu-shot-learning/page/211/

### Problem Statement

The goal is to predict how likely individuals are to receive their H1N1 and seasonal flu vaccines. Specifically, I'll be predicting ONLY one probability - h1n1_vaccine

### Data Cleaning/preparation
1. Checking the data structure, shape
2. Drop columns that had missing values >30%
3. Check for duplication

### Exploratory Data Analysis
- Quick Descriptive analysis of both categorical and numerical variables
- Visualize specific variables of importance to the exercise and check for relationship
-Engineer some columns

### Further Data Cleaning/preparation
- Replace missing based on context. 
- Create additional columns
- Further descriptive analysis to asess progress
### Data Analysis

``` Main notebook. Refer to H1N1 Classification Project.ipynb ;
```
### Results/findings
The analysis results are summarized as follows:
### Modeling
For this modeling exercise, I will focus on 
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - XGBoost
### Conclusion from Model Evaluations
- Our models could not achieve desirable results. 
- This being health related data, our goal would have to focuss on Recall(Sensitivity) so as not to miss out on any opportunity that had H1N1 and wrongly classified. 
- This implies we had many sick patients misclassified as healthy.In all, the recall was way too low and this can not help in making the correct prediction.
- As earlier mentioned above during EDA, we noticed the imbalance and this is what makes this model not to perform any better. 
This is because the model tends to predict the most occuring value in our target variable.

### Recommendations
- Use the SMOTE (Synthetic Minority Over-sampling Technique) approach to handle our imbalanced dataset.

- More can be read on how to go about this issue and whether more complex model can be of any help in future.Our models could not achieve desirable results. 

