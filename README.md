# Solar Plant Analysis

## Problem Statement
The primary challenge was to prepare and preprocess the data acquired for the year 2023 and establish a pipeline capable of handling data for any other year. This involved merging multiple Excel files, cleaning, and standardizing the data, handling missing values and outliers, aligning data discrepancies, and integrating the processed data into Power BI for further analysis to gain insights into solar plants and identify high and low performing plants.

## Approach
A systematic approach was adopted to address the challenges, including data acquisition, compilation, preprocessing, filtering, handling missing values and outliers, model training, quality control, segmentation, and integration. Each step was meticulously executed to ensure the accuracy and reliability of the data. A Regression Model was trained to predict POA Energy values, successfully predicting values for 93% of days.

## Predicted Outcome
The predicted outcome of the project was to have clean, standardized, and properly aligned data ready for analysis. Additionally, a regression model trained to predict POA energy was expected to provide valuable insights into energy production. An interactive dashboard was envisioned, allowing users to analyze specific sectors of plants using multiple filters such as Zone, State, City, OM Vendor, Investor, Panel Make, Type of Plant, Plant Owner, Capacity, and Month.

## Tools Used
- Excel
- Python (Pandas, NumPy)
- Power BI

## Project Steps
1. **Data Acquisition:** Obtained data for the year 2023.
2. **Data Compilation:** Merged all relevant Excel files into a single comprehensive file.
3. **Data Preprocessing:** Cleaned and standardized the data to ensure accuracy and consistency.
4. **Filtering:** Excluded non-essential data, retaining only specific types of plants.
5. **Exclusion Criteria:** Removed plants lacking inverters and meters, excluded rows with zero POA energy, and omitted data from specific plants.
6. **Handling Missing Values:** Filled missing values in 'meters' and 'inverters' columns, ensuring other columns had no missing values.
7. **Data Standardization:** Converted the date column to datetime format.
8. **Handling Outliers:** Replaced extreme values with the mean for respective plants.
9. **Data Alignment:** Addressed discrepancies in meter/inverter values and capacities.
10. **Model Training:** Utilized regression models to train for predicting POA energy.
11. **Quality Control:** Recalculated performance ratio (PR) and yield.
12. **Data Segmentation:** Created separate columns for inverters and meters, establishing distinct dataframes for energy values.
13. **Additional Information Inclusion:** Incorporated capacity, city, and state columns into the dataframes.
14. **Quality Assurance:** Eliminated entries with negative energy values and calculated PR and yield for each meter/inverter.
15. **Correct Panel Make Names:** Standardized panel make names for consistency.
16. **Integration:** Integrated processed data into Power BI, creating four separate files for plant details, plant energy, meter data, and inverter data.

## Actual Outcome
The project resulted in clean, standardized data ready for analysis and visualization in Power BI. The regression model provided insights into POA energy prediction, facilitating further analysis and decision-making. All the mentioned filters were successfully implemented. Four separate dashboards were created to analyze solar plants effectively: one for the entire portfolio, one for specific states, one for specific cities, and one for individual plant analysis, focusing on identifying the best performing meters and inverters.
