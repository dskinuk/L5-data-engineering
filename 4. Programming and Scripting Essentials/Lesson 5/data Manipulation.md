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
 - CSV files
 - SQL databases
 - Excel files
 - 
