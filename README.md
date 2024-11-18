# **Job Posting Analysis: Power BI Project**

## **Overview**
This project analyzes job postings in the U.S. tech sector using data from Kaggle. It provides insights into job trends, required skills, seniority levels, and company characteristics. The Power BI dashboard aims to help job seekers, companies, and recruiters make informed decisions about hiring and career planning.

---

## **Project Objectives**
- Clean and preprocess job posting data for accurate analysis.
- Identify in-demand skills, seniority levels, and popular job types.
- Provide actionable insights for job seekers and businesses.
- Highlight trends in remote versus on-site work and company sizes.

---

## **Key Features**
- **Interactive Dashboard**:
  - Filters for job type, location, company size, and skills.
  - Visualizations of job trends, top skills, and industry dynamics.
- **Insights**:
  - Top 10 most in-demand skills in the U.S. tech sector.
  - Seniority levels required for various roles.
  - Remote work trends and company size breakdowns.

---

## **Data Source**
- **Dataset**: Job postings data from Kaggle.
- **Fields Analyzed**: Job titles, company names, locations, job types, number of applicants, skills, and salaries.

---

## **Tools and Technologies**
- **Data Preparation**: Power Query (data cleaning and transformation).
- **Data Modeling**: DAX (Data Analysis Expressions) for calculations and measures.
- **Visualization**: Power BI for interactive dashboards and insights.

---

## **Data Cleaning and Transformation**
1. **Column Adjustments**:
   - Removed irrelevant columns like `Job Title Additional Info` to focus on actionable data.
   - Addressed missing values in `Number of Applicants` by replacing nulls with zero.
   - Dropped rows with missing values in critical fields like `Company Name`.
2. **Derived Fields**:
   - Created a `Job Status` column to categorize roles as Remote or On-Site.
   - Extracted `Job Location State` from the `Job Location` column and replaced ambiguous values (e.g., "US") with "Unknown."
3. **Job Skills Table**:
   - Split the `Job Skills` column to separate individual skills.
   - Removed unnecessary characters and cleaned text using TRIM and CLEAN functions.
   - Removed 2,210 blank rows to ensure data consistency.
4. **Categorization**:
   - Grouped `Company Size` into three categories: Startup, Medium-Sized, and Large.
5. **Date Table**:
   - Created a custom date table with columns for quarters, months, and days for time-based analysis.

---

## **Key Insights**
1. **In-Demand Skills**: Identified the top 10 skills employers seek.
2. **Remote Work Trends**: Highlighted the increasing demand for remote job roles.
3. **Job Seniority Levels**: Found significant demand for senior and expert-level roles.
4. **Company Types**: Analyzed the distribution of job postings by company size.
5. **Regional Trends**: Visualized hiring trends across different U.S. states.

---

## **Challenges and Solutions**
- **Challenge**: Managing missing and inconsistent data in key columns.
  - **Solution**: Applied appropriate cleaning techniques and removed irrelevant or duplicate entries.
- **Challenge**: Handling complex skill data with multiple entries.
  - **Solution**: Used splitting and transformation techniques to analyze individual skills effectively.

---

## **Next Steps**
- Expand the analysis to include industries beyond the U.S. tech sector.
- Incorporate real-time job posting data using APIs.
- Refine the data model with additional fields like salary analysis and career paths.

---

## **How to Use**
1. Download the Power BI file (`JobPostings.pbix`) from this repository.
2. Open the file in Power BI Desktop.
3. Explore insights using interactive filters and visualizations.

---

## **Target Audience**
- **Job Seekers**: Understand in-demand skills and job trends.
- **Recruiters**: Benchmark hiring trends and identify skill gaps.
- **Companies**: Align job postings with market trends and competitor standards.

---

## **Acknowledgments**
Special thanks to Kaggle for the dataset and contributors who assisted in data preprocessing and modeling.
