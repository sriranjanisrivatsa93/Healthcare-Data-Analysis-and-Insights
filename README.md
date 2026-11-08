# Healthcare Data Analysis & Insights

Objective: Clean and consolidate a 2,335-patient healthcare dataset in Excel to uncover cost drivers and risk patterns behind hospital charges.

## KPI snapshot
| KPI | Value |
|---|---:|
| Total patients | 2,335 |
| Average age | 40.09 |
| Average BMI | 30.97 |
| Average HbA1C | 6.58 |
| Total healthcare charges | $31,592,358.61 (~$31.6M) |
| Average healthcare charges | $13,529.92 (~$13.5K) |
| Smokers | 20.9% |
| Patients with transplants | 6.17% |
| Patients with cancer history | 16.75% |
| Patients with heart issues | 39.66% |

## Key findings
- **Obesity + Diabetes** patients had the highest average charges: **$19,347.66** (next highest: Obesity/Prediabetes at $15,353.90, Obesity/Normal at $15,188.44).
- Age correlates most strongly with **HbA1C (r = 0.46)** and **charges (r = 0.30)**, guiding cost-reduction targeting for high-risk segments.
- Top states by average charges: Unknown ($20,996.53), R1011 ($19,466.25), R1017 ($14,806.11).
- Most common weight category: **Obesity**; most common diabetes category: **Normal**; most frequent hospital tier: **Tier 2**.

## What was done
- Cleaned and standardized raw patient records in Excel/Python — resolved missing values, standardized categorical fields, derived age, weight-status, and diabetes-status indicators.
- Built pivot-based KPI tables and a slicer-driven interactive Excel dashboard covering charges by weight status, diabetes status, hospital tier, and state.

## Files
- `healthcare_assignment_completed.xlsx` — completed workbook with cleaning, transformation, analysis tables, and dashboard.
- `assignment_report.md` — detailed write-up of methodology and findings.
- `Module End Assignment 1_Excel - Healthcare Analysis and Insights.pdf` — exported report/screenshots.
