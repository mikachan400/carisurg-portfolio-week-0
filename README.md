# CariSurg Portfolio (Week 0)

This repository documents my progress during Week 0 of the CariSurg MedTech Pathways Programme, focusing on clinical data processing.

## 📌 Overview
This week focuses on developing foundational skills in clinical data processing, including setting up tools such as Google Colab, Python, and GitHub, and performing initial data exploration, cleaning and producing clinically meaningful visualisations. It also introduces basic exploratory data analysis (EDA) on a sample emergency department triage dataset.

## 🎯 Objectives
- Set up a working environment (Colab + GitHub)
- Load and explore a clinical dataset using Python
- Create basic and clinically meaningful visualisations to aid patient assessment
- Understand and explain key clinical vital signs
- Develop a simple rule to identify at-risk patients

## 🛠️ Tools Used
- Python (Google Colab)
- Pandas
- Matplotlib
- GitHub

## 📊 Dataset
The dataset used is a reduced, anonymised emergency department triage dataset containing patient demographics and vital signs.

**Note:** The dataset contains intentionally "dirty" values (inconsistent formats, invalid entries, and out-of-range values) to simulate real-world clinical data issues.

## ✅ Week 0 Progress

- Completed environment setup using Google Colab and GitHub
- Loaded and explored a clinical triage dataset
- Cleaned the Gender column into a consistent numerical format (1 = Male, 0 = Female)
- Performed advanced data cleaning on multiple clinical columns (GCS, SBP, Temperature, and Pulse)
- Applied clinical reference ranges to identify and handle invalid values
- Used median imputation to handle missing data
- Wrote a clinical paragraph describing pulse, including its definition, normal and abnormal ranges, and its importance in triage
- Submitted clinical paragraph as a PDF document via Google Drive
- Wrote an additional clinical paragraph on blood glucose as a vital sign not included in the dataset, explaining its clinical function, normal range, abnormal conditions, and importance in triage decision-making
- Submitted additional clinical paragraph as a PDF document via Google Drive
- Designed a digital triage algorithm using pseudocode to process patient data and categorise patients into risk levels based on clinical thresholds, ensuring all parameters were evaluated and the highest risk level was assigned

### 📊 Data Visualisation (Clinical Focus)
- **Temperature Histogram:** Visualised the distribution of patient temperatures, highlighting thresholds for hypothermia (<36.0°C) and pyrexia (>38.0°C), which are important for identifying potential sepsis cases.
- **MAP vs Pulse Scatter Plot:** Compared mean arterial pressure and heart rate to identify patterns associated with compensatory physiological responses, including potential shock states.

## 🧹 Cleaning Approach
For each clinical column, I followed a structured data cleaning process:
- Inspected values using unique values and summary statistics
- Converted data types to numeric format
- Applied clinical reference ranges to identify invalid values
- Replaced invalid values with NaN
- Used median imputation to handle missing data
- Verified results after cleaning

Clinical reference ranges were based on tutorial guidance and standard physiological limits.

## 🚀 How to Run
1. Open the notebook in Google Colab
2. Ensure `EmergencyTriageDataset_Reduced_Dirty.csv` is uploaded to your Colab environment or mount your Google Drive to match your environment pathing: `/content/drive/MyDrive/ColabNotebooks/`
3. Run all cells from top to bottom
4. The outputs will display cleaned data and summaries

## 📊 Clinical Visualisation Dashboard

Below are the key diagnostic plots generated from the cleaned triage data, mapping patient distributions against critical care thresholds:

| 1. Temperature/Sepsis Screening | 2. Hemodynamic Shock Tracking |
| :---: | :---: |
| <img src="temperature_sepsis_histogram.png" width="400" alt="Body Temperature Distribution Chart"> | <img src="map_vs_pulse_scatter.png" width="400" alt="MAP vs Pulse Scatter Plot"> |
| **Temperature Histogram:** Tracks patients crossing pyrexia (>38°C) and hypothermia (<36°C) lines. | **MAP vs. Pulse Scatter:** Highlights high-acuity patients landing in the upper-left shock crosshair. |

## 👤 Author
Shamika Glasgow
