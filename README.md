# Analysis on Company Attrition Rate

## 🔗 Project Links
- [Data Cleaning on Jupyter Notebook](https://app.datacamp.com/workspace/w/a1d227d0-4a94-4a0b-92ea-35eba9d6dc94)
- [Interactive Dashboard on Tableau](https://public.tableau.com/views/HRAnalytics_16845123839020/ExecutiveSummary?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

## 📖 Background
In this first ever BI competition, you will be exploring a dataset for a fictitious software company called Atlas Labs. You'll have to import, analyze, and visualize the data using Tableau.

The end goal will be a clean, self-explanatory, and interactive dashboard for the HR team of Atlas Labs. By conducting a thorough exploratory data analysis and creating visualizations, you'll dive deeper into attrition and what factors impact attrition. This analysis will help the organization determine what action they will need to take to retain more employees.

## 💾 The data

#### Your team created the following files:


### Employee (`employee.csv`)
|   Column name  |   Description | 
|---------------|-----------|
| Employee ID |	A unique ID that identifies an employee, connects to the **Performance Rating** table  |
|FirstName | First name of an employee  |
|LastName |	Last name / surname of an employee |
|Gender| Self-defined employee gender identity|
|Age|Current age of an employee|
|BusinessTravel|Frequency of business travel|
|Department | Most recent department that employee belongs/belonged to |
|DistanceFromHome (KM)|Kilometer distance between an employee’s home and their office|
|State|State where the employee lives|
|Ethincity| Self-defined employee ethnicity|
|Education | A unique ID that identifies an employees education level, connects to the **Education Level** table |
|EducationField|Employee field of study|
|JobRole |	Most recent department that employee belongs/belonged to |
|MaritalStatus|Current/latest employee marital status|
|Salary | Most recent record of employee salary |
|StockOptionLevel|The banding level for stock options that the employee has|
|OverTime|Indicates whether an employee is expected to work overtime in their role|
|HireDate|Date the employee joined the company|
|Attrition|Indicates whether an employee has left the organization|
|YearsAtCompany|Number of years since the employee joined the organization|
|YearsInMostRecentRole|Number of years the employee has been in their most recent role|
|YearsSinceLastPromotion|Number of years since the employee last got promoted|
|YearsWithCurrManager|Number of years the employee has been with their current manager|

### Performance Rating (`performance_rating.csv`)
|   Column name  |   Description | 
|---------------|-----------|
| PerformanceID | A unique id that identifies a performance review|
| EmployeeID |	A unique ID that identifies an employee, connects to the **Employee** table  |
|ReviewDate | Date an employees' review took place  |
|EnvironmentSatisfaction |	Rating for employees' satisfaction with their environment  |
|JobSatisfaction |	Rating for employees' satisfaction with their job role |
|RelationshipSatisfaction|Rating for employees' satisfaction with their relationships at work|
|WorkLifeBalance|Rating for employees' satisfaction with their relationships at work|
|SelfRating|Rating for employees' performance based on their own view|
|ManagerRating|Rating for employees' performance based on their manager’s view|
|TrainingOpportunitiesWithinYear|Number of training opportunities offered in the last 12 months|
|TrainingOpportunitiesTaken|Number of training opportunities taken|

### Education Level (`education_level.csv`)
|   Column name  |   Description | 
|---------------|-----------|
| Education Level ID | A unique id that identifies a education level
| Education Level |	A unique ID that identifies an employee, connects to the **Employee** table|

### Cleaned Merged Dataset 1 (`cleaned_data.csv`)
- A merged dataset consists of Employee Table, Performance Rating Table, and Education Level Table that has duplicates and errors removed.

### Cleaned Merged Dataset 2 (`unique_employeeId_data.csv`)
- A similar dataset to Cleaned Merged Dataset 1 but only consists of unique employee ID.


## 🔍 Executive Summary

1. Atlas Lab has hired 1217 employees since 2013 and 224 employees had left the company. Currently, there are 933 active employees and the average age of the employees in the company is around 30 years old, which is considered relatively young.

2. The total attrition rate for the company from 2013 to 2022 is 18.41% and Sales Department has the highest attrition rate of 24.18%, followed by Human Resources (HR) department and Technology department which had 22.64% and 15.50% attrition rate, respectively. However, the attrition rate has been decreasing since Year 2013 from a high rate of 84.38% to 19.77% on Year 2022.

3. From year 2013 to 2022, employees between the age 18 to 31 has the highest attrition rate of around 24%. Within this age range, employees with Doctorate or Masters education level are getting lesser salary compared to High School graduates in Sales and HR department. 

4. Data Scientists, Sales Executives, Software Engineers, and Sales Representatives quit the job is likely due to working over time requirement. Out of 88 sales department employees who have left the company, 47 employees required to work over time. Out of 12 HR department employees who have left the company, 5 employees required to work over time. Due to the need to work over time, employees are 50% likely to take up training opportunities.

5. Recommended actions to reduce attrition:
    - Increase the salary of employees who have high education level in Sales and HR department.
    - Allows hybrid working to improve work life balance, especially for employees who are married.
    - Reduce the workload on job roles that often need to work over time.
    - Encourage employees to enrol in training courses for upgrading their skillsets.

![Executive Summary](https://github.com/yirongNg/Data-Viz-on-Company-Attrition-Rate/assets/132359604/5a838492-3f02-48ec-b8db-60cba6d1165c)


