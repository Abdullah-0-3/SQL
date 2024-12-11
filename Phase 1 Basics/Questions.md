# Question - Basics SQL

### Question 1: Retrieve All Columns
Retrieve all columns for all records from the table information.

**Input Description:**
You need to write a SQL query to fetch all the data from the information table.

**Example Output:**
| id  | first_name | last_name  | department              | gender | email                    | salary    | country   | city         | family_members | car   | job_title           | date_of_birth | project_count |
|-----|------------|------------|-------------------------|--------|--------------------------|-----------|-----------|--------------|----------------|-------|---------------------|---------------|---------------|
| 1   | Vassili    | Barfield   | NULL                    | Male   | vbarfield0@cbsnews.com   | $8958.13  | Israel    | Hod HaSharon | NULL           | NULL  | NULL                | 2001-10-16    | 686           |
| 2   | Riannon    | McCloid    | Business Development    | Female | rmccloid1@jiathis.com    | NULL      | France    | Vannes       | 3              | NULL  | NULL                | 2007-09-18    | 240           |
| 3   | Rodrigo    | Nodin      | Research and Development| Male   | rnodin2@sun.com          | $6957.33  | Cambodia  | Kampong Speu | NULL           | Lexus | Environmental Tech  | 1991-09-17    | 259           |

---
### Question 2: Filter by Country
Write a query to retrieve the first_name, last_name, and country of all individuals where the country is 'France'.

**Input Description:**
- Filter the records where country is 'France'.
- Return only the first_name, last_name, and country columns.

**Example Output:**
| first_name | last_name | country |
|------------|-----------|---------|
| Riannon    | McCloid   | France  |

---
### Question 3: Filter by Salary
Write a query to retrieve all columns for individuals whose salary is greater than $8000.

**Input Description:**
- Filter the records where the salary column is greater than $8000.
- Return all columns from the table.

**Example Output:**
| id  | first_name | last_name  | department | gender | email                  | salary    | country | city         | family_members | car   | job_title | date_of_birth | project_count |
|-----|------------|------------|------------|--------|------------------------|-----------|---------|--------------|----------------|-------|-----------|---------------|---------------|
| 1   | Vassili    | Barfield   | NULL       | Male   | vbarfield0@cbsnews.com | $8958.13  | Israel  | Hod HaSharon | NULL           | NULL  | NULL      | 2001-10-16    | 686           |

---
### Question 4: Count the Records
Write a query to count the total number of records in the information table.

**Input Description:**
- Use an aggregate function to count the rows in the table.
**Example Output:**
| total_records |
|---------------|
| 3             |

---
### Question 5: Retrieve Unique Job Titles
Write a query to fetch all unique job_title values from the information table.

**Input Description:**
- Return a list of distinct job_title values.
**Example Output:**
| job_title           |
|---------------------|
| NULL               |
| Environmental Tech |

---