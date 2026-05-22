# CariSurg Portfolio (Week 0)

This repository documents my progress during Week 0 of the CariSurg MedTech Pathways Programme.

## Basic Overview
This week focuses on setting up the core tools and workflows required for clinical data work, including Google Colab, Python, and GitHub. It also introduces basic exploratory data analysis (EDA) on a sample emergency department triage dataset.

## Objectives
- Set up a working environment (Colab + GitHub)
- Load and explore a clinical dataset using Python
- Create basic visualisations
- Understand and explain key clinical vital signs
- Develop a simple rule to identify at-risk patients

## Tools Used
- Python (Google Colab)
- Pandas
- Matplotlib
- GitHub

## Dataset
The dataset used is a reduced, de-identified emergency department triage dataset containing patient demographics and vital signs.

Note: The dataset contains intentionally "dirty" values (inconsistent formats, invalid entries, and out-of-range values) to simulate real-world clinical data issues.

## Week 0 Progress
- Completed environment setup using Google Colab and GitHub
- Loaded and explored a clinical triage dataset
- Cleaned the Gender column into a consistent numerical format (1 = Male, 0 = Female)
- Performed advanced data cleaning on multiple clinical columns (GCS, SBP, Temperature, and pulse)
- Applied clinical reference ranges to identify and handle invalid values
- Used median imputation to handle missing data


## Cleaning Approach
For each clinical column, I followed a structured data cleaning process:
- Inspected values using unique values and summary statistics
- Converted data types to numeric format
- Applied clinical reference ranges to identify invalid values
- Replaced invalid values with NaN
- Used median imputation to handle missing data
- Verified results after cleaning

Clinical reference ranges were based on tutorial guidance and standard physiological limits.

## How to Run
1. Open the notebook in Google Colab
2. Upload the dataset file:
   EmergencyTriageDataset_Reduced_Dirty.csv
3. Run all cells from top to bottom
4. The outputs will display cleaned data and summaries

## Author
Shamika Glasgow 
