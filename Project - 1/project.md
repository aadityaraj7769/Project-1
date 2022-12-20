# *Build a model in machine learning that predicts whether the person would have survived the Titanic Shipwreck.*

## Target Variable -> Survived

1) Import important libraries -> 
    <br>
    numpy      -> for fundamental scientific computations like to create arrays or matrices.
    <br>
    pandas     -> for data wrangling and data manipulation purposes.
    <br>
    sklearn    -> for modeling like using logisticRegression and train test split
    <br>
    matplotlib -> for data visualization and graphical plotting
    <br>
    seaborn    -> it is for visualization library which has some plots like count plot, scatter plot, etc.

2) Read the file (or data).

3) Look over the data using "head" that will show the top 5 data.

4) Checking its size.

5) Looking about the information of data using ".info()" and here information means its datatypes and we can also see if there is any missing values in any features.

6) Checking only its datatypes.

7) Using "describe" we can get the information of all numerical features like its total count, mean, median, std. deviation, min, max, 25%ile, 75%ile, etc.

8) Using ".isnull().sum()" we will get the number of missing values in each column.

9) and 10) Analyse the data using sns.countplot 
 
11) and 12)

13) There's a lot of missing values in "Cabin" column so it is better to drop that column.

14) There's little missing values in "Age" and "embarked" column so I dropped the rows which has the missing values.

Now we have data in columns which is categorical but our computer is not capable to understand the categorical data so Now I will do one hot encoding 
Like first we do create its dummies and then replace the categorical data into its respective dummies in original datasets.
<br>
And we dropped column which is not correlated to the target variable like "PassengerId" Column.
<br>

Now I will implement the ML algorithm (Logistic Regression) and first we split the data into training and testing datasets. Basically I will take the 70% data into training dataset and remaining 30% into testing dataset.
I will build the model using training dataset and then checking the model with testing datasets and if the the model is neither underfitting nor overfitting then I can say that my model is perfect.