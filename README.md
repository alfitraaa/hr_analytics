# HR Analytics Project - Employee Attrition Analysis

## Objective
This project aims to analyze employee attrition data for a fictitious software company called **Atlas Labs**. The goal is to explore and visualize the factors that impact attrition and understand what actions can be taken to retain more employees. The project uses Tableau for data analysis and visualization to create a clean, self-explanatory, and interactive dashboard for the HR team of Atlas Labs.

## Dataset Description
1. **Employee** (employee.csv)
  - Employee ID:	A unique ID that identifies an employee, connects to the Performance Rating table
  - FirstName:	First name of an employee
  - LastName:	Last name / surname of an employee
  - Gender:	Self-defined employee gender identity
  - Age:	Current age of an employee
  - BusinessTravel:	Frequency of business travel
  - Department:	Most recent department that employee belongs/belonged to
  - DistanceFromHome (KM):	Kilometer distance between an employee’s home and their office
  - State:	State where the employee lives
  - Ethincity:	Self-defined employee ethnicity
  - Education:	A unique ID that identifies an employees education level, connects to the Education Level table
  - EducationField:	Employee field of study
  - JobRole:	Most recent department that employee belongs/belonged to
  - MaritalStatus:	Current/latest employee marital status
  - Salary:	Most recent record of employee salary
  - StockOptionLevel:	The banding level for stock options that the employee has
  - OverTime:	Indicates whether an employee is expected to work overtime in their role
  - HireDate:	Date the employee joined the company
  - Attrition:	Indicates whether an employee has left the organization
  - YearsAtCompany:	Number of years since the employee joined the organization
  - YearsInMostRecentRole:	Number of years the employee has been in their most recent role
  - YearsSinceLastPromotion:	Number of years since the employee last got promoted
  - YearsWithCurrManager:	Number of years the employee has been with their current manager

2. **Performance Rating** (performance_rating.csv)
  - PerformanceID:	A unique id that identifies a performance review
  - EmployeeID:	A unique ID that identifies an employee, connects to the Employee table
  - ReviewDate:	Date an employees' review took place
  - EnvironmentSatisfaction:	Rating for employees' satisfaction with their environment
  - JobSatisfaction:	Rating for employees' satisfaction with their job role
  - RelationshipSatisfaction:	Rating for employees' satisfaction with their relationships at work
  - WorkLifeBalance:	Rating for employees' satisfaction with their relationships at work
  - SelfRating:	Rating for employees' performance based on their own view
  - ManagerRating:	Rating for employees' performance based on their manager’s view
  - TrainingOpportunitiesWithinYear:	Number of training opportunities offered in the last 12 months
  - TrainingOpportunitiesTaken:	Number of training opportunities taken

3. **Education Level** (education_level.csv)
  - Education Level ID:	A unique id that identifies a education level
  - Education Level:	A unique ID that identifies an employee, connects to the Employee table

## Project Steps:

- **Data Preprocessing**: The first step involves data preprocessing in Python (Google Colab). Data cleaning, wrangling, and anomaly detection are performed to prepare the data for further analysis.

- **Exploratory Data Analysis**: Using Tableau, we conduct a thorough exploratory data analysis (EDA) on the cleaned data. We create visualizations to gain insights into attrition, job satisfaction, work-life balance, and its connect them with another dimensions.

- **Dashboard Creation**: The final output is an interactive dashboard created in Tableau. The dashboard includes various visualizations, such as bar charts, KPIs, pie chart and heatmaps, to showcase the key findings and trends related to attrition and its impacting factors.

## Conclusion:
Through my analysis I obsereved that in recent year the number or people leaving the company had been on the rise. But let us look more into why people leave. Based on the analysis, the following conclusions can be drawn:

1. **Attrition Rate:** The attrition rate for the company is 18.41%, indicating that approximately 18.41% of employees have left the company.

2. **Employee Age:** The age group with the highest number of employees is between 22 to 27 years, with a total of 560 employees.

3. **Department Analysis:** Technology department has the lowest attrition rate of employees compared to the other two departments, accounting for 15.5% of the total workforce.

4. **Average Satisfaction:** The average satisfaction level from the conducted surveys is 3.44 out of 5, indicating a moderate overall satisfaction among employees.

5. **Key Factors for Attrition:** The analysis shows that the key factors contributing to increased attrition are "Travel Frequency" and "Overtime." This trend is consistent across all departments, indicating that employees who travel frequently and work overtime are more likely to leave the organization.

## Recommendations:

Based on the findings, the following recommendations can be made to address the attrition issue:

1. **Employee Engagement:** Focus on enhancing employee engagement programs to improve job satisfaction and work-life balance.

2. **Flexible Work Arrangements:** Offer flexible work arrangements to reduce the impact of frequent business travel and overtime, promoting a better work-life balance.

4. **Exit Interviews:** Conduct exit interviews with departing employees to gain insights into the reasons for attrition and identify areas for improvement.

5. **Review Workload and Staffing:** Conduct a thorough assessment of the workload and staffing requirements in each department. If certain departments or teams consistently experience high overtime demands, it may indicate that the workload is not adequately distributed or that additional resources are needed. Consider hiring more staff or redistributing tasks to balance the workload and reduce the need for excessive overtime.

6. **Set Realistic Deadlines:** Collaborate with project managers and team leaders to set realistic deadlines for projects and tasks. Unrealistic deadlines can put immense pressure on employees, leading to extended work hours and burnout. Ensuring that deadlines are achievable will help mitigate the need for excessive overtime.

## Closing

Thank you for your interest in this HR Analytics project focused on employee attrition analysis for Atlas Labs. Through data preprocessing, exploratory data analysis, and visualization using Tableau, we gained valuable insights into attrition rates, employee satisfaction, and key factors influencing attrition.

I appreciate any suggestions and feedback you may have to improve the analysis and visualization further. This project serves as a learning experience, and I welcome any input to enhance future data analytics projects.

**Project Resources:**
1. **Google Colab:** [Google Colab Link](https://colab.research.google.com/drive/1vrqW-IPVcm-6LbV43XDG1ZaoCHDTQ4RO?usp=sharing)
2. **LinkedIn Profile:** [LinkedIn Profile Link](https://www.linkedin.com/in/farizalfitra/)
3. **Tableau Public:** [Tableau Link](https://public.tableau.com/views/HRAnalyticsDashboard_16908071863670/Dashboard?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

The dataset used for this analysis is available in the project's GitHub repository. By sharing this project and its resources, I hope it can help anyone who might want to try it yourself or anyone who interested in People Analytics. Feel free to explore the Tableau dashboard and the dataset to gain deeper insights into the analysis.

Thank You.
