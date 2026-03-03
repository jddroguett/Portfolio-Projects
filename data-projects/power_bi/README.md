# Power BI – Data Professional Survey Analysis

## Project Overview
This project analyzes a dataset of data professionals to explore career paths, salaries, industries, and other demographic factors. The workflow uses Power BI and follows a structured data preparation and cleaning process.

## Data Source
- **File:** `Power BI - Final Project.xlsx`  
- **Sheet:** `Data Professional Survey`  
- Contains survey responses including role, salary, programming language, industry, happiness metrics, and demographics.

## Data Cleaning & Transformation
The following steps were applied in Power Query:

1. **Load Source**: Imported the Excel sheet into Power BI.  
2. **Promote Headers**: Converted the first row of the sheet into column headers.  
3. **Change Data Types**: Assigned appropriate types to columns (text, date, time, numeric).  
4. **Remove Unnecessary Columns**: Dropped irrelevant fields such as `Browser`, `OS`, `City`, `Country`, and `Referrer`.  
5. **Split Columns**:  
   - Role titles and programming languages were split to isolate the main text.  
   - Extra parts were removed to simplify analysis.  
6. **Clean Salary Data**:  
   - Duplicated salary column for processing.  
   - Removed non-numeric characters (`k`, `-`, `+`) and standardized values.  
   - Calculated `Average Salary` from numeric parts.  
7. **Reorder and Rename Columns**: Organized columns for readability and renamed temporary columns.  
8. **Clean Industry & Country Columns**: Removed extra information in parentheses, keeping only the main value.

## Output
- Cleaned dataset ready for analysis in Power BI visualizations.  
- Columns include:  
  - Unique ID, Email, Date/Time Taken, Time Spent  
  - Role, Career Switch, Current Salary, Average Salary  
  - Industry, Favorite Programming Language  
  - Happiness Metrics (Salary, Work/Life Balance, Coworkers, Management, Upward Mobility, Learning)  
  - Difficulty Breaking into Data, Job Priorities, Gender, Age, Country, Education, Ethnicity

## Dashboard
Using this cleaned dataset, a **Power BI dashboard** was created to visualize key insights, including:  
- Salary distributions and averages by role and industry  
- Career paths and industry trends  
- Happiness and work/life balance metrics  
- Demographics and survey responses  
This dashboard provides an interactive overview of the dataset and supports exploratory analysis.

## Notes
- All transformations are documented in the Power Query Editor.  
- This setup ensures the dataset is consistent, numeric fields are clean, and categorical data is standardized, ready for visual dashboards or further analysis.

