# COVID-19 Wearables Data Exploration

Exploratory data analysis of the **Welltory COVID-19 and Wearables Open Data Research dataset**.  
This project demonstrates how to work with messy, real-world health data collected from wearable devices during the COVID pandemic.

## Project Overview
The dataset contains anonymized heart rate variability (HRV) and related metrics collected via the Welltory app.  
My analysis focuses on:
- Understanding and documenting key features (`user_code`, `measurement_datetime`, `rmssd`, `pnn50`, etc.)
- Cleaning and standardizing data for reliable analysis
- Handling missing values, duplicates, and outliers
- Performing transformations (e.g., datetime parsing, extracting `date` and `hour`)
- Visualizing distributions and trends in HRV measures
- Assessing data quality (completeness, accuracy, consistency, integrity, provenance)

## Key Steps
1. **Feature Understanding** – explained columns and dataset context.  
2. **Cleaning** – imputed missing HRV values with medians, clipped outliers at 1st–99th percentile, removed duplicates by (`user_code`, `measurement_datetime`).  
3. **Transformation** – converted datetime fields and engineered new `date` and `hour` features.  
4. **Visualization** – histogram of RMSSD, daily RMSSD line trends, scatter plots (steps vs HRV if present).  
5. **Data Quality Discussion** – completeness, sampling bias, and lineage of the Welltory dataset.

## Repository Contents
- `hadil_week4_exploration.ipynb` → Jupyter notebook with full analysis  
- `README.md` → Project description and summary  

## Reflection
This project reinforced that **data cleaning choices directly shape downstream insights**.  
Working with a messy, observational dataset highlighted challenges like incomplete features and outlier noise — exactly the type of real-world complexity analysts and data scientists face outside of clean classroom datasets.

---

### Step 3: Commit and push README
```bash
git add README.md
git commit -m "Add README with project overview"
git push origin main
