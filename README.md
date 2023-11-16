# Crimes-against-women-in-India

1. **Importing Libraries:**
   - The script starts by importing necessary libraries, including Pandas for data manipulation and analysis, NumPy for numerical operations, and Seaborn/Matplotlib for data visualization.

2. **Loading the Dataset:**
   - The script reads a CSV file named 'crimes_against_women_2001-2014.csv' into a Pandas DataFrame (`df`).

3. **Data Exploration:**
   - The script displays the first few rows of the dataset using `df.head()` to provide an overview of the data.
   - It checks for information about the dataset using `df.info()`.

4. **Handling Missing Values:**
   - The script checks for missing values in the dataset using `df.isnull().sum()`.

5. **Data Cleaning:**
   - Columns 'DISTRICT' and 'Unnamed: 0' are dropped from the DataFrame using `df.drop`.
   - Column names are standardized by renaming them using `df.rename`.

6. **Data Transformation:**
   - The 'STATE/UT' column values are converted to uppercase and leading/trailing whitespaces are removed using a custom function (`remove_upper`).

7. **Data Standardization:**
   - Standardizing state/union territory names by replacing specific values using `df['STATE/UT'].replace`.

8. **Summary:**
   - The code aims to prepare the dataset for analysis by cleaning, transforming, and standardizing the data.
