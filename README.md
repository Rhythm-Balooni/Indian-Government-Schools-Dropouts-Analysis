# School Enrollment and Facilities Analysis in India

This project performs a comprehensive analysis of school enrollment and facilities data in India, focusing on gender disparities and sanitation facilities. The analysis is spread across multiple datasets containing information on primary, middle, and high schools, and visualizes the relationships through various plots.

## Overview
This project aims to analyze the following:
1. Enrollment trends across different school grades
2. Fractional decrease in enrollments per class
3. Availability of sanitation facilities in schools
4. Correlation between sanitation facilities and the retention rate of girls from Class I to Class X

## Datasets
The analysis uses the following datasets:
1. `primary_rural_urban.xls`: Enrollment data for primary schools.
2. `middle_school_rural_urban.xls`: Enrollment data for middle schools.
3. `9_10_rural_urban.xls`: Enrollment data for high schools.
4. `facilities_primary.xls`: Sanitation facilities data for primary schools.
5. `facilities_secondary.xls`: Sanitation facilities data for secondary schools.
6. `facilities_upper_primary.xls`: Sanitation facilities data for upper primary schools.
7. `school_category.xls`: Total number of schools and their categories.

Analysis Steps
1. Data Import and Merging: Import datasets and merge them based on the STATE/U.T. column.
2. Data Processing: Clean the data by stripping whitespace from column names and renaming columns for consistency.
3. Enrollment Data Analysis:
   - Initialize an empty dataframe for enrollment data. Loop over different class levels to extract and append enrollment data.
   - Plot the enrollment data and calculate the fractional decrease in enrollments per class.
5. Facilities Data Analysis: Combine the number of usable toilets from primary, secondary, and upper primary schools.
6. School Category Data Analysis:
   - Calculate the total number of schools excluding higher secondary schools.
   - Create a dataframe to store overall schools, schools with toilets, and the fraction with toilets.
8. Girls Retention Analysis: Calculate the fraction of girls retained from Class I to Class X and add it to the data frame.
9. Correlation and Plotting:
   - Calculate the correlation between the fraction of schools with toilets and the fraction of girls retained.
   - Plot a scatter plot of the fraction of schools with toilets versus the fraction of girls retained.

Results
1. Plots showing students enrolled in different classes in India.
2. Plots showing the fractional decrease in enrollments per class.
3. Scatter plot showing the correlation between the fraction of schools with toilets and the fraction of girls retained from Class I to Class X.
