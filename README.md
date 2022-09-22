# OUI-Bootcamp-CAPSTONE-PROJECT
<img width="1500" alt="Home Page (3)" src="https://user-images.githubusercontent.com/105246702/191678163-73098cce-45e3-4fce-a2ae-a68fe11e2711.png">

# Problem Satement
  The Palmoria Group, a manufacturing company based in the Nigeria is embroiled in issues bordering on gender inequality in its 3 regions. Unfortunately, the media recently published in the news with the headline “Palmoria, the Manufacturing Patriarchy” This doesn’t look good for the owners of the business based on their ambition to scale the business to other regions and even overseas. Cases like this can only spiral downwards revealing other issues like gender pay gap amongst other possible issues.

  As an HR Analytics expert, I was assigned the task to analyze the company’s HR data to identify key areas within the business that could spring up issues and come up with recommendations for management’s attention and give a breakdown of the Salary details.

  “Now, the future of gender equality in Palmoria lies in your hands” the exact words of Mr. Shofoluwe before he handed the data to me.

# Objective
● Focus is on gender related issues within the organization and its regions
1. Gender distribution in the organization
2. Insights on ratings based on gender
3. Company’s salary structure. To identify if there is a gender pay gap. If there is, the department and regions that should be the focus of management.
4. If Palmoria meets the requirement of manufacturing companies paying employees a minimum of #90,000
5. Pay distribution of employees grouped by a band of #30,000.
5. Allocation of the annual bonus pay to employees based on the performance rating.
- Amount to be paid as bonus to individual employees
- Total amount to be paid to individual employees (salary inclusive of bonus)
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

⚠ N.B: The undisclosed gender category may affect the accuracy of this analysis. However, they make up for only about 4% of the total employees.

### Gender Distribution
  ● General Overview

There is a total of 943 employees, 464 Males, 440 Females and 39 undisclosed.

<img width="128" alt="GENDER DISTRIBUTION" src="https://user-images.githubusercontent.com/105246702/191838029-7f508b4e-c330-4485-9605-fea0f34817ee.png">

Gender distribution is fair in the company with Males being 2% more than females and about 4% of employees did not disclose their gender.

<img width="190" alt="overall gender distribution" src="https://user-images.githubusercontent.com/105246702/191838078-6918e522-1704-4436-a85f-a586f395935d.png">

  ● Regions
  
Abuja has a balanced proportion of Males and Females with 158 each.

Kaduna is the region with the widest gender gap with 18 more Males than Females.

Lagos also has more 6 Males than Females.

<img width="185" alt="GENDER DISTRIBUTION by region" src="https://user-images.githubusercontent.com/105246702/191838182-e08dd2a8-02f3-419d-8ca6-ac728274c979.png">

  ● Department
  
Legal, Accounting, Support, Research and developemtent and Product Management are the top 5 departments with the most gender gaps each with a gap difference of 15,9,8,7,6 difference respectively.

In Marketing, Engineering and Training it's fairly distributed with gap of 2,2, 1 respectively

Futher Analysis shows that of the Top 5 departments with most gap, Research and developemtent is the only department where the Females are more than Males, the remaning 4 have more males.
Other departments with more females are Services, business development, Human Resources, Engineering.

<img width="201" alt="GENDER DISTRIBUTION by department" src="https://user-images.githubusercontent.com/105246702/191838285-06e8bbff-215d-42e4-b2a8-ab7ae53aa427.png">


### Rating
Rating was fairly distibuted among the genders.

Males had more very poor,poor and average rating while females lead in the good and very good category

<img width="381" alt="Rating by gender" src="https://user-images.githubusercontent.com/105246702/191838392-4a6f2a63-4235-4d00-9d17-288205de283f.png">


### Salary
  ● General Overview
  
Total Salary to be Paid out by the company is #71.74M incuding bonus, bonus salary is about #2.19M and salary without bonus is #69.54M

The average salary is #73,747

<img width="115" alt="salary company" src="https://user-images.githubusercontent.com/105246702/191838457-72752c48-795f-4e07-8059-0dc62229cee0.png">

Average salary among the genders is fairly distributed

<img width="191" alt="average salary" src="https://user-images.githubusercontent.com/105246702/191838746-addf82c3-3eaf-4db6-9c90-23cb23a82ad1.png">

  ● Regions
  
Kaduna Total Salary is #24.79M, Abuja is #27.42M and Lagos Total Salary is #19.53M

<img width="187" alt="salary regional" src="https://user-images.githubusercontent.com/105246702/191838574-e9a43293-621c-4ae8-ac03-920a84366f28.png">

  ● Department
  
In most departments, the Males earn more except 3 departments where females earn more Training, Marketing and Engineering

<img width="187" alt="Salary department" src="https://user-images.githubusercontent.com/105246702/191838825-a2532190-144c-428d-ab98-e0b4136d1315.png">

  ● Salary Range
  
Grouping the salaries by a band of #30k. Most employees earn within the range 61k to 90k, and least earn within 1k to 30k.

<img width="207" alt="salary range" src="https://user-images.githubusercontent.com/105246702/191840470-fd663365-f28d-4e37-9030-c9f48413242b.png">

  ● Minimum Salary requirment
  
There was a recent regulation which requires manufacturing companies to pay employees a minimum of #90,000.

Palmoria group falls short of this, with about 69% of the workers earning less than the minimum requirment

<img width="183" alt="90k" src="https://user-images.githubusercontent.com/105246702/191842435-1afd415c-fb20-414a-b9ed-82df8ca13362.png">

# Findings
•	Gender is fairly distributed throughout the organization

•	Average salary is close for both gender categories but there are far more men than women earning between $110,000 - $120,000

•	Employees ratings are fairly distributed across the genders

•	Majority of the employees earn salaries below the minimum requirement 


# Recommendation
•	The salaries should be reviewed upwards for the entire organization to ensure the minimum salary requirement is met.

•	The salary gap between men and women earning between $110,000 - $120,000 should be reviewed for fairness.

•	Gender distribution should be improved in Kaduna region and across Legal, Support, Sales, and Accounting departments.









