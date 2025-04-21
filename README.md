# 📊 Data Analyst Internship — Task 1

## 🔍 Task: Data Cleaning and Preprocessing  
**Dataset:** Netflix Movies and TV Shows  
**Tool Used:** Python (Pandas)


## ✅ Objective
To clean and preprocess a raw dataset by handling missing values, duplicates, inconsistent formats, and ensuring uniformity in structure for further analysis.


## 🛠 Steps Performed

### 📥 Loaded the Dataset
- Used `pandas.read_csv()` to load the dataset.

### 🏷 Renamed Columns
- Cleaned column names by converting to lowercase and replacing spaces with underscores.

### ❌ Handled Missing Values
- Dropped rows with missing `title`, `director`,
- Replaced missing values in `cast`, `country`, and `date_added` with `'Unknown'`.

### 🔁 Removed Duplicates
- Used `drop_duplicates()` to remove identical rows.

### 🗓 Standardized Date Format
- Converted `date_added` column to `dd-mm-yyyy`.

### ⏱ Parsed Duration
- Extracted numeric values from `duration` into a new column `duration_parsed`.


## 📂 Files Included

- `netflix_titles.csv` — Raw dataset  
- `cleaned_netflix_data.csv` — Final cleaned dataset  
- `netflix_cleaning_script.py` — Python script used for preprocessing  
- `README.md` — This documentation file  


## 🧠 Concepts Practiced

- Handling missing values with `.isnull()`, `.fillna()`, `.dropna()`  
- Removing duplicates with `.drop_duplicates()`  
- Date formatting using `pd.to_datetime()`  
- Feature engineering (`duration_parsed` column)  
- Data type and format standardization  


## 🧾 Sample Output Preview

| show_id | type    | title | director | cast       | ... | date_added | release_year | duration   | duration_parsed |
|---------|---------|-------|----------|------------|-----|------------|--------------|------------|-----------------|
| s1      | TV Show | 3%    | Unknown  | Joao M...  | ... | 14-08-2020 | 2020         | 4 Seasons  | 4               |

