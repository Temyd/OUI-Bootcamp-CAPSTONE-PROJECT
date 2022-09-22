# OUI-Bootcamp-CAPSTONE-PROJECT
<img width="1500" alt="Home Page (3)" src="https://user-images.githubusercontent.com/105246702/191678163-73098cce-45e3-4fce-a2ae-a68fe11e2711.png">

# Introduction
“Now, the future of gender equality in Palmoria lies in your hands” the exact words of Mr. Shofoluwe before he handed the data to me.

# Objective
● Focus is on gender related issues within the organization and its regions
1. Gender distribution in the organization? Distil to regions and departments
2. Insights on ratings based on gender
3. Company’s salary structure. To identify if there is a gender pay gap. If there is, the department and regions that should be the focus of management.
4. If Palmoria meets the requirement of manufacturing companies paying employees a minimum of $90,000
5. Pay distribution of employees grouped by a band of $10,000.  How many employees fall into a band.
5. Allocation of the annual bonus pay to employees based on the performance rating.
- Calculate the amount to be paid as bonus to individual employees
- Calculate the total amount to be paid to individual employees (salary inclusive of bonus)
- Total amount to be paid out per region and company-wide


# Data Sourcing

# Data Transformation
● I loaded the employee dataset into Power Query it had 6 columns 1016 rows
● I assigned a generic gender status (Undisclosed) to employees that refused to disclose their gender.
● I removed employees without salary (because they are no longer with the company), departments that indicated as “NULL”. I also removed duplicates from the dataset thus giving us 6 columns 943 rows
● I had to get the bonus salary for each employee,so I loaded the bonus details dataset which had 6 columns and 12 rows. I unpivoted the rating columns givng me a total of 3 columns and 60 rows after which I then merged both the bonus details and employee details together using department and rating column. Leaving us with 7 columns 943 rows. (Since I merged already, I disabled the bonus dataset from loading into powerbi)
● I then loaded into powerbi desktop 
● I created some new measures to help in my analysis
● I also created a new column 'Salary Ranges' to group the salaries in a band of 10k
● 
● 

# Data Visualisation

# Analysis

### Gender Distribution


