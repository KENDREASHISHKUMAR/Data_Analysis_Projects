# Dataset Description  

* The Titanic dataset is a well-known dataset in the field of machine learning and data science. It contains real-world data from the infamous RMS Titanic disaster, which occurred on April 15, 1912, after the ship struck an iceberg. The dataset includes details about passengers, ticket information, class, fare, age, family relations, and survival status, making it a great resource for classification, statistical analysis, and predictive modeling.  

## General Information:  
* Total Entries: 891  
* Columns: 12  
* Missing Values:  
  - Age: 177 missing values.  
  - Cabin: 687 missing values (highly sparse).  
  - Embarked: 2 missing values.  

## Column Overview:  
* PassengerId: Unique identifier for each passenger.  
* Survived: Survival status (0 = No, 1 = Yes).  
* Pclass: Ticket class (1st, 2nd, 3rd).  
* Name: Passenger’s full name.  
* Sex: Gender of the passenger (male/female).  
* Age: Age of the passenger (range: 0.42 - 80 years).  
* SibSp: Number of siblings/spouses aboard.  
* Parch: Number of parents/children aboard.  
* Ticket: Ticket number.  
* Fare: Ticket fare (range: 0 - 512).  
* Cabin: Cabin number (mostly missing).  
* Embarked: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).  


# Data Preprocessing Steps  

## Loading the Dataset  
- The Titanic dataset is loaded using `pd.read_csv("train.csv")`.  

## Handling Missing Values  
- **Age**: 177 missing values are filled with the **mean age**.  
- **Embarked**: 2 missing values are filled with the **mode of the Embarked column**.  
- **Cabin**: Missing values are imputed based on **survival status and class**:  
  - For **survivors** in **1st, 2nd, and 3rd class**, missing cabins are filled with `"B96"`.  
  - For **non-survivors** in **1st, 2nd, and 3rd class**, missing cabins are filled with `"C23"`.  

## Encoding Categorical Variables  
- Categorical variables such as `Sex`, `Cabin`, `Embarked`, and `Pclass` are converted into dummy variables using `pd.get_dummies()`.  
- The original categorical columns are **dropped after encoding**.  

## Dropping Unnecessary Columns  
- Columns that are **not needed** for the analysis, such as `Name`, `PassengerId`, and `Ticket`, are **dropped** from the dataset.  

## Feature and Target Variable Separation  
- The **feature set (X)** is created by **dropping the `Survived` column**.  
- The **target variable (y)** is set to the **`Survived` column**.  

## Train-Test Split  
- The dataset is split into **training and testing sets** using `train_test_split()` with a **test size of 30%**.  






# Titanic Dataset Analysis Insights

## Model Results
- **Accuracy Score**: The logistic regression model achieved an accuracy score of approximately **0.95** (95%) on the test dataset.

### Classification Report
- The classification report includes metrics for each class (Survived: 0 and 1):
  - **Precision**: Ratio of correctly predicted positive observations to the total predicted positives.
  - **Recall**: Ratio of correctly predicted positive observations to all actual positives.
  - **F1-Score**: Weighted average of Precision and Recall.
  - **Support**: Number of actual occurrences of the class in the specified dataset.

### Confusion Matrix
- Displays the true positives, true negatives, false positives, and false negatives.

## Visualisation Insights
### Survival Rate Observations
- Only ~38% of passengers survived, while ~62% perished.
- Women had a much higher survival rate (~74%) compared to men (~18%).
- Children (age < 10) had a better chance of survival than adults.

### Gender and Survival Insights
- ~74% of females survived, while only ~18% of males survived.
- The “Women and children first” policy led to a higher survival rate for women.
- Male survival was much lower, especially in 3rd Class (~13%).

## Summary
- Higher class, higher fare, and being female or a child greatly increased survival chances.
- Men in 3rd class had the worst survival rate (~13%).
- Passengers with large families struggled to survive.

# Conclusion
The analysis of the Titanic dataset provides valuable insights into the factors affecting survival during the disaster, with clear correlations between class, age, and survival rates.
