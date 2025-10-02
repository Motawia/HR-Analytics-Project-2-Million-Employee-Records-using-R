# HR-Analytics-Project-2-Million-Employee-Records-using-R
Overview

This project analyzes Human Resource (HR) data from a multinational corporation (MNC) containing 2 million employee records.
The dataset includes employee demographics, job-related attributes, salary details, performance ratings, and employment status.

The goal is to perform HR analytics using R and answer 15 key business questions on workforce distribution, attrition, performance, salary trends, and hiring patterns.

The analysis combines data wrangling, statistical tests, and visualizations to deliver actionable insights for HR.

🔗 Dataset Source

The dataset used in this project is publicly available on Kaggle:
👉 HR Data Complete Analysis – Kaggle

🔍 Key Analyses (Q1–Q15)

Distribution of Employee Status (Active, Resigned, Retired, Terminated)

Distribution of Work Modes (On-site vs Remote)

Number of Employees in Each Department

Average Salary by Department

Job Title with the Highest Average Salary

Average Salary by Department & Job Title

Resigned & Terminated Employees per Department

Salary vs. Years of Experience (with and without outliers)

Average Performance Rating by Department

Country with the Highest Employee Concentration

Correlation between Performance Rating and Salary

Hiring Trends Over Time (per year)

Salary Comparison: Remote vs On-site (t-test + effect size)

Top 10 Highest Paid Employees in Each Department

Departments with the Highest Attrition Rate (Resigned %)

🛠️ Technologies Used

R Programming

Statistical Analysis (t-test, effect size, correlation)

Data Visualization (bar charts, pie charts, boxplots, line plots, scatter plots, maps)

📚 Libraries
library(gridExtra)     # arrange multiple plots together
library(dplyr)        # data manipulation
library(tidyverse)    # data science toolkit (includes ggplot2, dplyr, etc.)
library(stringr)      # string handling (extract countries)
install.packages("rworldmap")
library(rworldmap)    # world map visualization
install.packages("countrycode")
library(countrycode)  # convert country names to ISO codes
library(lubridate)    # work with dates (hire year)
library(scales)       # format numbers (commas, percentages)
install.packages("effsize")
library(effsize)      # effect size (Cohen’s d, Hedges’s g)

# Turn off scientific notation globally
options(scipen = 999)

📊 Visualizations

The project generates multiple plots:

Bar charts and pie charts for categorical distributions

Boxplots to analyze salary & performance variation

Line plots for trends (salary vs experience, hiring per year)

Scatter plots with regression lines to check correlations

Faceted charts for department-level insights

Geographic maps for employee distribution by country

 How to Run

Clone the repository:

git clone https://github.com/motawia/hr-analytics.git


Open RStudio and install required packages:

install.packages(c("gridExtra", "dplyr", "tidyverse", "stringr",
                   "rworldmap", "countrycode", "lubridate", "scales", "effsize"))


Load the dataset (CSV with 2M rows).

Run HR_Analysis.R step by step (Q1–Q15).

📈 Results

Salary distribution and performance vary across different departments.

Attrition rates highlight the most vulnerable departments.

Remote vs On-site employees show no significant salary difference (confirmed by statistical tests and effect size).

Hiring trends reveal key workforce expansion periods.
