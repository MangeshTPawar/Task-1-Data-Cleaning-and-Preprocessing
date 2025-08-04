# Task-1-Data-Cleaning-and-Preprocessing

This notebook performs data cleaning and preprocessing on student performance data from two datasets: student-mat.csv and student-por.csv.

Steps Performed:

Load Data: The student-mat.csv and student-por.csv files were loaded into pandas DataFrames.

Merge Data: The two dataframes were merged into a single dataframe named std based on common columns.

Check for Null Values: The merged dataframe was checked for null values, and no null values were found.

Check for Duplicate Values: The merged dataframe was checked for duplicate rows, and no duplicate rows were found.

Standardize Text Values: Text values in object columns were converted to lowercase and leading/trailing whitespace was removed for consistency.

Identify Numerical and Categorical Columns: Columns were separated into numerical and categorical types for further analysis and preprocessing.

Analyze Numerical Columns: Descriptive statistics and box plots were used to analyze the distribution and identify potential outliers in numerical columns.

Handle Numerical Outliers: Outliers in the 'absences' and 'failures' columns were capped at the 95th percentile, and outliers in the grade columns ('G1_x', 'G2_x', 'G3_x', 'G1_y', 'G2_y', 'G3_y') were capped at the valid range of [0, 20].

Analyze Categorical Columns: Value counts were used to check for inconsistent or rare categories in categorical columns.
