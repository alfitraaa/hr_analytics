# HR Analytics Project - Employee Attrition Analysis

## Objective
This is a legacy educational HR / People Analytics project demonstrating Python preprocessing, multi-table data handling, data-quality checks, employee vs review grain separation, descriptive attrition analysis, and Tableau visualization. It analyzes descriptive employee attrition data for a fictitious software company called **Atlas Labs**.

## Dataset Description
1. **Employee** (`Datasets/employee.csv`)
    - Employee ID: A unique ID that identifies an employee, connects to the Performance Rating table (Note: contains one corrupted ID `0.00E+00` appearing across 3 records).
    - FirstName: First name of an employee
    - LastName: Last name / surname of an employee
    - Gender: Self-defined employee gender identity
    - Age: Current age of an employee
    - BusinessTravel: Frequency of business travel
    - Department: Most recent department that employee belongs/belonged to
    - DistanceFromHome (KM): Kilometer distance between an employee’s home and their office
    - State: State where the employee lives
    - Ethincity: Self-defined employee ethnicity
    - Education: A unique ID that identifies an employees education level, connects to the Education Level table
    - EducationField: Employee field of study
    - JobRole: Employee's specific job role/title
    - MaritalStatus: Current/latest employee marital status
    - Salary: Most recent record of employee salary
    - StockOptionLevel: The banding level for stock options that the employee has
    - OverTime: Indicates whether an employee is expected to work overtime in their role
    - HireDate: Date the employee joined the company
    - Attrition: Indicates whether an employee has left the organization
    - YearsAtCompany: Number of years since the employee joined the organization
    - YearsInMostRecentRole: Number of years the employee has been in their most recent role
    - YearsSinceLastPromotion: Number of years since the employee last got promoted
    - YearsWithCurrManager: Number of years the employee has been with their current manager

2. **Performance Rating** (`Datasets/performance_rating.csv`)
    - PerformanceID: A unique id that identifies a performance review
    - EmployeeID: A unique ID that identifies an employee, connects to the Employee table
    - ReviewDate: Date an employees' review took place
    - EnvironmentSatisfaction: Rating for employees' satisfaction with their environment
    - JobSatisfaction: Rating for employees' satisfaction with their job role
    - RelationshipSatisfaction: Rating for employees' satisfaction with their relationships at work
    - WorkLifeBalance: Rating for employees' satisfaction with their relationships at work
    - SelfRating: Rating for employees' performance based on their own view
    - ManagerRating: Rating for employees' performance based on their manager’s view
    - TrainingOpportunitiesWithinYear: Number of training opportunities offered in the last 12 months
    - TrainingOpportunitiesTaken: Number of training opportunities taken

3. **Education Level** (`Datasets/education_level.csv`)
    - Education Level ID: A unique id that identifies a education level
    - Education Level: Descriptive education level string

## Project Steps:

- **Data Preprocessing**: Preprocessing in Python (Jupyter Notebook). Data cleaning, data-quality checks, separation of employee and performance review grains, and formatting. You can run the notebook from the repository root:
  ```bash
  pip install pandas scikit-learn jupyter
  jupyter notebook HR_Analytics.ipynb
  ```

- **Exploratory Data Analysis**: Descriptive data analysis to gain insights into attrition distributions and observed group differences.

- **Dashboard Creation**: The final output is an interactive dashboard created in Tableau. The dashboard includes various visualizations to showcase descriptive findings and trends related to attrition.

## Conclusion:
Based on the full-workforce analysis, the following descriptive conclusions can be drawn:

1. **Attrition Prevalence:** 237 of 1,470 employee records are marked Attrition = Yes, or 16.12% of the employee snapshot.
2. **Employee Age:** There are 619 employee records in the 22 to 27 years age bracket.
3. **Department Analysis:** Technology department has the lowest observed attrition prevalence at 13.84%. It accounts for 961 records (65.37% of the total workforce). Sales has an attrition prevalence of 20.63% and Human Resources 19.05%.
4. **Satisfaction:** The datasets contain multiple separate review-level satisfaction metrics (Environment, Job, Relationship, Work-Life Balance). These are best evaluated descriptively across individual performance reviews rather than as a single synthetic company-wide number.
5. **Observed Group Differences:** Descriptive analysis shows that frequent travellers have a higher observed attrition prevalence (24.91%) compared to employees with some travel (14.96%) or no travel (8.00%). Additionally, employees reporting overtime have a higher observed attrition prevalence (30.53%) compared to those without overtime (10.44%).

*(Note: There is no statistical causal design or predictive attrition model here. These are descriptive associations, and confounders are not controlled.)*

## Questions for Further Investigation:

Based on the observed descriptive patterns, the following questions could be investigated further:

1. **Travel Impact:** Why is observed attrition prevalence higher among frequent travellers?
2. **Overtime Context:** Are overtime patterns associated with specific roles, teams, or tenure groups?
3. **Workload and Flexibility Interventions:** Would flexible-work or workload interventions reduce attrition? This would require separate evaluation to determine causal impact.
4. **Exit Feedback:** What do exit interviews indicate about reasons for leaving?

## Closing

Thank you for your interest in this HR Analytics project. Through Python data preprocessing and Tableau visualization, it demonstrates multi-table data handling and descriptive employee attrition analysis.

**Project Resources:**
1. **Tableau Public:** [Legacy Tableau Link](https://public.tableau.com/views/HRAnalyticsDashboard_16908071863670/Dashboard?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)
   > *Legacy Tableau dashboard: this visualization was built from the original preprocessing pipeline and has not yet been revalidated against the corrected employee-grain pipeline. The notebook and README in this repository are the current analytical source of truth.*

Feel free to explore the dataset and the notebook to gain deeper insights into the descriptive analysis.
