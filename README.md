The dataset underwent the following cleaning and preprocessing steps:
Initial Data Inspection
Loaded the dataset using pandas.

Inspected the shape, data types, and a few sample rows using head(), info(), and describe() functions.
Handling Missing Values
Identified and analyzed missing values using isnull().sum().

Filled missing values in specific columns with placeholders or using imputation strategies (e.g., mode or zero).

Date Parsing
Converted date columns (like date_added) to datetime format using pd.to_datetime(), ensuring proper temporal analysis.
Splitting and Converting Columns

For columns like duration, used regular expressions to split into:
duration_int: numeric part (converted to integer)
duration_type: unit (e.g., 'min', 'Seasons')
Converted extracted duration values to numeric using pd.to_numeric() with error handling.

Duplicate and Irrelevant Data
Checked for and removed any duplicate entries using drop_duplicates().

Standardizing Text
Cleaned string columns by:
Stripping whitespace

Feature Engineering 
Created new columns or transformed existing ones for better usability (e.g., extracting year from date, categorizing durations).

Final Check
Confirmed there are no nulls or inconsistent data types left.
