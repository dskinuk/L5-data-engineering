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

## Sorting, grouping, aggregating data
df. sort_values()
df. group_by()
- Group by 'Condition' - grouped_data = df groupby('Condition' )
- Aggregate to find the average age by 'Condition' - aggregated_data = grouped _data['Age'] - mean(
- Display the grouped  DataFrame - print("Aggregated DataFrame:"); print(aggregated_data)
- grouping multiple cols - grouped_multi = df groupby(['Condition', 'Hospital'])

- Aggregating - summarising or transforming the grouped values - aggregated_data = grouped_data[ 'Age']. mean()
- 
  
## Merge/Join/concat
- merge() - allows you to combine DataFrames in a manner similar to SQL joins. e.g. merged_inner = pd.merge(df_temp, df_prec, on='Date')
- join() - easier to use than merge() and combines DataFrames based on indices by default or you can provide a key as a parameter
joined_left = df_temp.join(df_prec, Isuffix='_temp', ruffixe'_prec', how= 'left')
- concat() - combines DataFrames along a particular axis, either row-wise (axis=0) or column-wise (axis=1), without needing any keys.
  concatenated = pd.concat([df_temp, df_wind], ignore_index=True)
  
## REGEX - ??
