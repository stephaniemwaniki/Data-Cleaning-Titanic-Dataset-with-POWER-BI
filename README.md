# DATASET: Titanic dataset
[Titanic Data.xlsx](https://github.com/stephaniemwaniki/Data-cleaning-Titanic-Dataset-with-POWER-BI/files/10944000/Titanic.Data.xlsx)
# Dataset Overview
I did data cleaning on the Titanic dataset which comprises of information about 891 passengers who were in the Titanic ship that sank in 1912.
The dataset is made up of the following columns:
- PassengerId - Id of all 891 passengers.
- Pclass - The passenger class each passenger was in the ship.
- Name - Name of the passengers.
- Sex - Gender of the passengers.
- Age - Age of the passengers.
- SibSp - The number of siblings and spouses each passenger has.
- Parch - The number of parents and children each passenger has.
- Ticket – Ticket number of each passenger.
- Fare – Fare each passenger paid in US Dollars.
- Cabin – Cabin number of each passenger.
- Embarked – Where each passenger embarked on the ship.
- Survived - If the passenger survived or not.
# Data Cleaning
Data cleaning was done using Power BI. The tasks involved were:
-  Cleaning Pclass column
by changing values 1, 2, 3 to 1st class, 2nd class, 3rd class respectively and renamed column to Passenger Class.            
Procedure: add column tab-column from examples-replace value then click CTRL+ENTER.
- Cleaning Name column
by splitting Name column into three columns namely Title, Other names and Surname.
Procedure: surname was first separated by transform tab-split column-by delimiter “comma” “left most delimiter” options then title was separated from other names by transform tab-split column-by delimiter “.” “left most delimiter” options.
- Cleaning Sex column
by renaming Sex Column to Gender
- Cleaning SibSp and Parch columns
by forming new column “Family size” by merging these columns.
Procedure: add column tab-custom column-enter new column name “Family size” and custom column formula = [SibSp] + [Parch] + 1.
- Cleaning Ticket column
by removing extra spaces in all records in Ticket column.
Procedure: add column tab-format-trim.
- Cleaning Embarked column.
by replacing values S with Southampton, C with Cherbourg and Q with Queenstown.
Procedure: Select column-right click-click “replace value”-enter “value to find” and “replace with”
- Cleaning Survived column
by renaming it to Survival and replaced values 0 with died and 1 with survived.
Procedure: add column tab-column from examples-replace value then click CTRL+ENTER.
# New Dataset Overview
[Cleaned Titanic data.xlsx](https://github.com/stephaniemwaniki/Data-cleaning-Titanic-Dataset-with-POWER-BI/files/10944035/Cleaned.Titanic.data.xlsx)

The new dataset formed has the following columns:
- PassengerId
- Passenger class
- Title
- Other names
- Surname
- Gender
- Age
- Family size
- Ticket
- Fare
- Cabin
- Embarked
- Survival

