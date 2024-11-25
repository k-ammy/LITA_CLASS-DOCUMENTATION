# LITA_CLASS_DOCUMENTATION

### Project Title: Data Discovery: Documenting my Analytics Experience

[Project Overview](#project-overview)

[Data Sources](#data-sources)

[Tools Used](#tools-used)

[Data Cleaning and Preparation](#data-cleaning-and-preparation)

[Data analysis](#data-analysis)

[Data Visualization](#data-visualization)




### Project Overview
---
This project serves as a personal documentation of my journey as I transition into the field of data analysis. It covers my growth from learning fundamental concepts to working with real-world datasets and applying various data analysis techniques.The objective of this project is to track my progress, reflect on key learning milestones, and demonstrate my ability to solve data problems using analytical approaches. It also serves as a resource for those interested in understanding the process of transitioning into data analytics, particularly through self-learning and structured courses.

### Data Sources
---
The Primary source of Data used is Salary review.xlxs and this is an open source data that can be freely downloaded from an open source online such as kaggle or FRED or any other data repository site.

### Tools Used
---
- Microsoft Excel [Download Here](https://www.microsoft.com)
    1. Data Cleaning
    2. For Analysis
    3. For Visualisation
- SQL - Structured Query Language for Quering of Data
- GitHub for Portfolio Building

### Data Cleaning and Preparation
---
In the Data Cleaning and Preparation section of your documentation, you'll want to list out the common steps you follow to ensure the data is ready for analysis. Here's a structured list of key steps typically involved:
-    Data Importation:
        1. Load the raw data into a suitable environment (e.g., pandas DataFrame). Example: df = pd.read_csv('data.csv').
-    Handling Missing Data:
        1. Identifying missing values: Check for missing or NaN values using methods like isnull() or info().
-    Imputing or removing missing data:
        1. Drop missing values: df.dropna()
        2. Impute missing data (e.g., fill with mean, median, or a constant value): df.fillna(df.mean()).
-    Removing Duplicates:
        1. Identify and remove any duplicate rows or entries.
-    Handling Outliers:
        1. Detecting outliers: Use methods such as box plots or statistical techniques like z-score.
        2. Handling outliers: Remove or cap outliers based on business logic or statistical thresholds.
-    Correcting Inconsistent Data Types:
        1. Convert data types to their appropriate format (e.g., dates to datetime, numerical values to float or int).

### Exploratory Data Analysis
---
Exploratory Data Analysis (EDA) is a critical process in data analysis where you analyze and summarize the main characteristics of a dataset. It involves the use of statistical and visualization techniques to uncover patterns, spot anomalies, test hypotheses, and verify assumptions before applying more complex analytical models. EDA provides a deeper understanding of the data and helps you make informed decisions about data preprocessing and modeling. Key objectives of EDA are:
- Understand Data Structure: Examine the dataset’s size, shape, and structure, including the number of rows and columns, data types, and basic statistics.
- Detect Outliers: Identify unusual data points that could affect model performance.
- Find Missing Data: Uncover missing or incomplete data that needs to be handled.
- Discover Patterns: Spot trends, correlations, or groupings within the data.
- Test Hypotheses: Explore relationships between variables to validate assumptions.

### Data Analysis
---
This is where we include some basic line of code or query or some of DAX expressions used during my analysis;
- Data Analysis Expressions Using Microsoft Excel:
- 
```EXCEL
=SUM(A2:A10)
```
```EXCEL
=AVERAGE(B2:B10)
```
```EXCEL
=IF(A2>50, "Pass", "Fail")
```
```EXCEL
=COUNTIF(A2:A10, ">50")
```
```EXCEL
=SUMIF(B2:B10, ">50", C2:C10)
```
```EXCEL
=VLOOKUP(D2, A2:C10, 3, FALSE)
```
```EXCEL
=INDEX(B2:B10, MATCH(D2, A2:A10, 0))
```
```EXCEL
=LEFT(A2, 3)  // Extracts first 3 characters
```
```EXCEL
=RIGHT(B2, 4) // Extracts last 4 characters
```
```EXCEL
=LEFT(A2, 3)  // Extracts first 3 characters
```
```EXCEL
=RIGHT(B2, 4) // Extracts last 4 characters
```
```EXCEL
=A2 & " " & B2
```
```EXCEL
=TRIM(A2)
```
```EXCEL
=TODAY()
```
```EXCEL
=DATEDIF(A2, B2, "D")  // "D" for days
```

- Data Analysis Expressions Using Structured Query Language (SQL)

```SQL
SELECT column1, column2 FROM table_name;
```
```SQL
SELECT * FROM employees WHERE salary > 50000;
```
```SQL
SELECT SUM(salary) FROM employees;
```
```SQL
SELECT AVG(salary) FROM employees;
```
```SQL
SELECT COUNT(*) FROM employees;
```
```SQL
SELECT MIN(salary), MAX(salary) FROM employees;
```
```SQL
SELECT department, AVG(salary) FROM employees GROUP BY department;
```
```SQL
SELECT department, AVG(salary)
FROM employees
GROUP BY department
HAVING AVG(salary) > 50000;
```
```SQL
SELECT employees.name, departments.name
FROM employees
INNER JOIN departments ON employees.department_id = departments.id;
```
```SQL
SELECT employees.name, departments.name
FROM employees
LEFT JOIN departments ON employees.department_id = departments.id;
```
```SQL
SELECT * FROM employees ORDER BY salary DESC;
```
```SQL
SELECT name FROM employees WHERE salary > (SELECT AVG(salary) FROM employees);
```
```SQL
SELECT name, salary, 
CASE
  WHEN salary > 50000 THEN 'High'
  WHEN salary BETWEEN 30000 AND 50000 THEN 'Medium'
  ELSE 'Low'
END AS salary_category
FROM employees;
```

### Data Visualization

![PIVOT Chart](https://github.com/user-attachments/assets/38e28179-4420-470a-8044-153e828fcd64)

![583a08ee-fec1-49a7-b293-100cdd5fb1af (2)](https://github.com/user-attachments/assets/f64ec37b-2119-4b54-9f88-421449a0b565)

|Heading 1|Heading 2|Heading 3|
|---------|---------|---------|
|Table 1|Table 2|Table 3|
