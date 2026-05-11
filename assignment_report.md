# Healthcare Data Analysis Assignment - Submission Notes

## Generated Artifacts
- healthcare_assignment_completed.xlsx: Completed workbook with cleaning, transformation, merged healthcare data, analysis tables, and dashboard charts.
- assignment_solution.py: Reproducible script that builds the completed workbook from the original dataset.

## Data Cleaning Completed
- Counted missing values marked with ? in both Medical Examinations and Hospitalisation Details.
- Filled missing month with Sep.
- Filled missing year using rounded average: 1983.
- Filled missing smoker, Hospital tier, and City tier using mode values.
- Filled missing State ID with Unknown.

## Data Transformation Completed
- Split customer names into Title, First Name, and Last Name.
- Converted NumberOfMajorSurgeries to numeric values (No major surgery -> 0).
- Standardized yes/no categorical fields (Heart Issues, smoker, etc.).
- Added Weight Status based on BMI bands.
- Added Diabetes Status based on HBA1C bands.
- Created Date of Birth from year/month/date and formatted as DD-MMM-YYYY.
- Calculated Age as of 08-Jun-2023.
- Formatted charges as currency.

## Exploration and Visualization Completed
- Created consolidated Healthcare sheet with required columns using Customer ID key.
- Added analysis tables for:
  - Cancer history distribution among smokers/non-smokers.
  - Surgeries + average HBA1C by transplant status.
  - Average charges by Weight Status and Diabetes Status.
  - Average charges by State and Hospital tier.
  - Age correlation with BMI/HBA1C and age vs charges trend.
- Added dashboard charts in Dashboard sheet.

## How to Regenerate Output
Run: python assignment_solution.py
