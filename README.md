# Palmoria-Group-HR-Analysis
### Palmoria Group manufacturing company HR Analysis Project

## Overview
<p style="color: #FFFFFF; border-bottom: 1px solid #CCCCCC">The Palmoria Group, a manufacturing company in Nigeria, faces issues of gender inequality, prompting the CEO to assign the CHRO to lead an initiative to address these concerns. As an HR Analytics expert, I analyzed the company's HR data to identify key areas of concern and provide recommendations for management's attention.</p>

## Data Collected

The dataset includes the following key columns:

1. Name: The names of employees in the company
2. Gender: The genders of employees in Palmoria
3. Department: Department names in the company
4. Salary: Employee salaries in the company
5. Region: Regions where Palmoria company is located
6. Rating: Employee performance ratings
7. Department rating: Departmental ratings
8. Bonus rate: Employee bonus rates
9. Annual bonus: Annual bonuses paid to employees
10. Total pay: Total salary for each employee
11. Salary band: Salary categories for employees
12. Rating score: Numerical ratings for employee performance

    
## Project Objectives
1. Analyze gender distribution and inequality: Examine the company's employee data to identify potential biases or disparities in gender representation across departments and regions.
2. Evaluate performance ratings and potential biases: Investigate employee ratings based on gender to determine if there are any potential biases or disparities.
3. Assess salary structure and pay gaps: Analyze the company's salary structure to identify potential pay gaps between genders and determine which departments and regions require attention.
4. Determine compliance with minimum salary regulation: Evaluate the company's compliance with the recent regulation requiring a minimum salary of $90,000 and identify employees who may require salary adjustments.
5. Calculate bonus payments and total compensation: Calculate individual and total bonus payments based on performance ratings and determine the total compensation for each employee.
6. Provide recommendations for improvement: Based on the analysis, provide actionable recommendations to address identified issues, promote gender equality, and ensure a more inclusive and equitable work environment.

## Key Metrics
1. Gender Distribution Ratio: Percentage of male and female employees across the organization, departments, and regions.
2. Employee Performance Rating Distribution: Average performance ratings by gender, department, and region.
3. Pay Gap Ratio: Ratio of average salaries between male and female employees, overall and by department/region.
4. Minimum Salary Compliance Rate: Percentage of employees meeting the minimum salary requirement of $90,000.
5. Bonus Payment Distribution: Average bonus payments by performance rating, department, and region.
6. Total Compensation Package: Average total compensation (salary + bonus) by employee, department, and region.
7. Regional Employee Count: Number of employees by region.
8. Departmental Employee Count: Number of employees by department.
9. Salary Band Distribution: Number of employees in each salary band ($10,000 increments).
10. Return on Investment (ROI) for Bonus Payments: Analysis of the impact of bonus payments on employee performance and retention.

## Formula Used

Measure
- Gender Count = COUNT('Employee'[Gender])
- Gender Percentage = DIVIDE(CALCULATE(COUNT('Employee'[Gender])), CALCULATE(COUNT('Employee'[Gender]), ALL('Employee'[Gender])))
  
Measure
- Average Rating by Gender = AVERAGE('Employee'[Rating])
- Rating Count by Gender = COUNT('Employee'[Rating])

Measure 
- Average Salary by Gender = AVERAGE('Employee'[Salary])
- Salary Count by Department and Region = COUNT('Employee'[Salary])

Measure
- Employees Below Minimum Salary = COUNTX(FILTER('Employee', 'Employee'[Salary] < 90000), 'Employee'[Salary])

Measure
- Total Compensation = SUM('EMPLOYEE'[Salary]) + SUMX(FILTER('EMPLOYEE', 'EMPLOYEE'[Rating Score] = 4), 'EMPLOYEE'[Salary] * 0.1)

## Tools and Methods Used
- Data Analysis: The data was analyzed using Microsoft Power BI, utilizing custom column, conditional column and measures
- Data Visualization: An interactive dashboard was created in Microsoft Power Bi to illustrate trends and insights


## Key Insights

| Insight | Description |
| --- | --- |
| 1. Gender Distribution | Analysis of employee data reveals the gender distribution across the organization, regions, and departments. |
| 2. Ratings and Performance | Insights into employee ratings based on gender highlight potential biases or disparities. |
| 3. Salary Structure and Pay Gap | Analysis of the company's salary structure reveals a potential gender pay gap, with identification of departments and regions that require attention. |
| 4. Minimum Salary Requirement | Evaluation of the company's compliance with the recent regulation requiring a minimum salary of $90,000. |
| 5. Pay Distribution | Visualization of employee pay distribution grouped by bands of $10,000, including regional breakdowns. |


## Bonus Payment Analysis

| Analysis | Description |
| --- | --- |
| 1. Individual Bonus Payments | Calculation of bonus amounts for individual employees based on performance ratings. |
| 2. Total Compensation | Calculation of total amounts to be paid to individual employees, including salary and bonus. |
| 3. Regional and Company-Wide Bonus Payments | Calculation of total bonus payments per region and company-wide. |




## The Dashboard


![image alt](https://github.com/isaacayeni225/My-Daily-Expenses-Tracker/blob/648f7fa31f3f72aedaff654b6203519ed8ccb6ca/Screenshot%20(10).png)

![image alt](https://github.com/isaacayeni225/Palmoria-Group-HR-Analysis/blob/0fe0a4e88e7fe2f6a549ceaa6f4480a892ac65f7/Screenshot%20(16).png)



## Recommendations
Based on the analysis, recommendations will be provided to address the identified issues, including:

1. Addressing Gender Inequality: Strategies to promote gender equality and address biases in ratings and salary structures.
2. Salary Adjustments: Recommendations for salary adjustments to meet the minimum requirement and address pay gaps.
3. Bonus Payment Allocation: Guidelines for allocating bonus payments based on performance ratings.

## Conclusion
The Palmoria Group HR Analysis aims to provide a comprehensive understanding of the company's employee data, focusing on gender distribution, performance ratings, salary structure, and compliance with minimum salary regulations. By achieving the project objectives, this analysis will deliver actionable insights and recommendations to promote gender equality, address potential biases and pay gaps, and ensure a more inclusive and equitable work environment. The findings of this analysis will enable the Palmoria Group to make informed decisions, drive positive change, and foster a workplace culture that values diversity and promotes employee well-being.

