# Historical_Data_Transformation
Transform current employee data from a columnar format into a historical, row-based versioning format suitable for database storage using Python.
Steps for execution 

1.Reading CSV File:It reads a CSV file named 'input.csv' and loads it into a Pandas DataFrame called df.
2.Date Columns and Data Transformation:This list contains the column names that represent dates. The code then iterates through each row of the DataFrame, extracts effective dates, and creates historical records based on those dates. It creates a new DataFrame called transformed_df.
3.Performance Rating and Engagement Score Matching: The code matches performance ratings and engagement scores with their respective dates and creates new columns ('Performance Rating' and 'Engagement Score') in the transformed_df.
4.Identifying Last Compensation:It identifies the last compensation for each employee and creates a new DataFrame named last_compensation.
5.Merging Last Compensation with Transformed Data:It merges the last_compensation DataFrame with the transformed_df DataFrame based on the 'Employee Code' column.
6.Creating New 'Compensation' Column:It creates a new 'Compensation' column based on the available compensation columns.
7.Removing Duplicates and Unwanted Columns:It removes duplicates from the transformed_df and drops specified columns from the DataFrame. The result is stored in the variable df.
8.Displaying Result:It displays the first 20 rows of the final transformed DataFrame.
9.Expoting csv file output.csv


In summary, the code reads a CSV file, transforms the data by creating historical records based on effective dates, matches performance ratings and engagement scores, identifies the last compensation for each employee, and creates a new 'Compensation' column. Finally, it removes duplicates and unwanted columns, displaying the resulting DataFrame.


