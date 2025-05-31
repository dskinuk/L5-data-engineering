# Data Manipulation

## Intro to pandas
used in data manipulation, cleaning, transformation, analysis
Benefits :
- Performance - much faster than excel
- flexibility - more customised data maniplation than SQL
- Ecosystem - Versatile and better compatibility with other data analytic libraries (Numpy, SciPy etc)
- Large Datasets - overcomes excel's data sixe limitations
- Automation - enables reproducble pipelines

## Installing pandas
## Exploring data structures

- Series - Single dimensional data
import pandas as pd

  data = [10,20,30,40]
  my_series = pd.series(data)
  print(my_series)

- Dataframes - Two dimensional data
- pd.read_csv() - can be used to import a CSV file into the dataframe
- df.haed() - to display the top rows of data

## Importing data
 - CSV files - pd.read_csv()
 - SQL databases - pd.read_sql() 
 - Excel files - pd.read_excel()
## Exporting data
- df.to_csv()
- df.to_excel()
- df.to_sql()

## Data Cleaning
 - Missing Values - df['Name'].fillna('unknown', inplace = True). 
 - Duplicate values - drop_duplicate()
df drop_duplicates(subset=['Name', 'Age'], keep='first', inplace=True)
 - Inconsistent formats - df['Age'].fillna(df['Age'].median()).astype(int) - FIll missing values of age using the median function. And also ensuring the data type is integer.
 - Outliers - outliers = df[df['Age'] > 100] . To delete the row with outlier value, sumplay re-assign the resultant dataset to itself.
   df = df[df['Age'] <= 100]

## Data maniplation and subsetting
.loc[]
.iloc[]

- Adding or dropping columns from data frames
    - Conditional Adding - 
df['Stock_Status'] = ['Low' if x < 100 else 'High' for x in df['Stock_Level']]
print("DataFrame after adding new column:")
print (df)
- FIltering data
  filtered_df = df[df['Stock_Status'] == 'Low']
print("Filtered DataFrame:")
print(filtered_df)




 - 
