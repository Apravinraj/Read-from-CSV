# Read-from-CSV

## AIM:
To write a program for reading the csv file content.
## ALGORITHM:
### Step 1:
Load the CSV into a DataFrame

### Step 2:
Print the number of contents to be displayed using df.head().

### Step 3:
The number of row returned is defined in pandas option settings.

### Step 4:
Check your systems maximun column with the pd.options.display.max_columun statement

### Step 5:
Increase the maximum number of rows to display the entire DataFrame.

## PROGRAM:

```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Interact:",regr.intercept_)
print("Amount:",regr.predict([[3000,1300]]))
```
## OUTPUT:

![Screenshot 2023-06-09 184253](https://github.com/Apravinraj/Read-from-CSV/assets/118707879/2e47ffe8-0bd6-4492-bdb5-411c4358c104)

## RESULT:
Thus the program written to read csv file.
