**Student Academic Performance Analysis Dashboard**

**Project Overview**
This repository contains a comprehensive Power BI Dashboard designed to analyze and visualize student academic performance across multiple semesters. The project focuses on transforming raw academic data into actionable insights for educators and students, highlighting key trends, subject difficulty levels, and overall class performance.

**Key Features**
Dynamic Navigation: Seamlessly switch between semesters using a custom-built navigation menu.
KPI Tracking: Real-time calculation of Average GPA, Pass Percentage, and Total Students using advanced DAX measures.
Subject Analysis: * Grade Distribution: Stacked bar charts showing the spread of grades (O, A+, A, etc.) across subjects.
Success Rate: Comparison of "Appeared" vs "Passed" students per subject.
Statistical Insights: Scatter plots to identify GPA outliers and a Subject Difficulty Index based on grade averages.
Data Transformation: Leveraged Power Query to unpivot subject columns and clean data for efficient modeling.

**Tools & Technologies**
Visualization: Power BI Desktop
Data Processing: Power Query (M Language)
Calculations: DAX (Data Analysis Expressions)
Data Source: MS Excel (Structured Academic Records)

**DAX Measures Used**
A few examples of custom calculations implemented:
Pass %: DIVIDE(CALCULATE(COUNT(Grade), Grade <> "U"), COUNT(Grade), 0)
Fail Count: CALCULATE(COUNT(Grade), Grade = "U")
Subject-wise GPA: Dynamic average calculation based on weighted grade points.

**Dashboard Preview**

Semester 1 Analysis: Deep dive into subject-wise performance.

![](screenshots_of_dashboard/homepage.png)


**How to Use**

Download the .pbix file from this repository.
Open it using Power BI Desktop.
Navigate through the different tabs to explore the interactive visuals
