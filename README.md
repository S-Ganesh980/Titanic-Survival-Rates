# Titanic-Survival-Rates

We classify the survival of passengers on the Titanic using a simple Logistic Regression.

The dataset comprises of the following information about the passengers aboard the Titanic: 
<br>
  1. PassengerId: Passenger identification number <br>
  2. Survived: 0 indicates that the passenger did not survive and 1 indicates that the passenger did survive<br>
  3. Pclass: Passenger class- 1st, 2nd or 3rd<br>
  4. Name: Name of the passenger <br>
  5. Sex: Male or female<br>
  6. Age: Age of the Passenger<br> 
  7. SibSp: Number of Siblings or Spouses aboard<br>
  8. Parch: Number of Parents or children aboard <br>
  9. Ticket: Ticket number <br>
  10. Fare: Passenger fare <br>
  11. Cabin: Cabin the passenger was in <br>
  12. Embarked:  Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)<br>

We started by importing the dataset and doing some Exploratory Data Analysis(EDA). During the course of EDA, we figured that there were missing data points in the Age and Cabin columns. 
We then imputed the missing Age-values with the average age based on the Passenger class because we found a trend that the passengers in the first class were older than those in the second class ,and the passengers in the second class were older than those in the third class. 
We omitted the Cabin column because maximum data points were missing. We then converted the categorical variables (Age and Embarked) into dummy variables and omitted other columns which did not contribute to the model. 
A classification model with an accuracy of 82% was created using Logistic Regression. 
