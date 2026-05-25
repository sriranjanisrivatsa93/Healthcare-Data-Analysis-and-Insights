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
- In the Dashboard sheet, added analysis tables for:
  - Cancer history distribution among smokers/non-smokers.
  - Surgeries + average HBA1C by transplant status.
  - Average charges by Weight Status and Diabetes Status.
  - Average charges by State and Hospital tier.
  - Age correlation with BMI/HBA1C and age vs charges trend.
- Also created a slicer based interactive dashboard that can be used to change these charts.

## KPI snapshot
| KPI | Value |
|---|---:|
| Total patients | 2335 |
| Average age | 40.09 |
| Average BMI | 30.97 |
| Average HbA1C | 6.58 |
| Total healthcare charges | $31,592,358.61 |
| Average healthcare charges | $13,529.92 |
| Smokers | 20.9% |
| Patients with transplants | 6.17% |
| Patients with cancer history | 16.75% |
| Patients with heart issues | 39.66% |

## Analytical findings
The most common weight category in the cleaned dataset is **Obesity**, while the most common diabetes category is **Normal**. The most frequent hospital tier in the hospitalization records is **tier - 2**.

Patients in the highest charge combination among weight and diabetes segments are **Obesity / Diabetes** with average charges of $19,347.66. The next two highest segments are **Obesity / Prediabetes** at $15,353.90 and **Obesity / Normal** at $15,188.44.

For transplant history, the group labeled **No** recorded total major surgeries of 1417.0 and average HbA1C of 6.67, while the group labeled **yes** recorded total major surgeries of 162.0 and average HbA1C of 5.19.

The top three states by average healthcare charges are **Unknown** at $20,996.53, **R1011** at $19,466.25, and **R1017** at $14,806.11.

## Correlation insights
The correlation between age and BMI is 0.052, the correlation between age and HbA1C is 0.460, and the correlation between age and charges is 0.304. These values suggest how strongly age moves with body mass, diabetic risk, and treatment cost in the dataset used for the assignment.
