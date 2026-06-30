# Health Analytics Dashboard - Power BI

An interactive 2-page business intelligence dashboard analyzing body metric distributions across gender and age groups, built on a 10,000-record health dataset.

**[View Dashboard File (PBIX)](Health%20Analytics%20Dashboard%20-%20Power%20BI.pbix)**

![Dashboard Overview](Health%20Overview.png)
![Detailed Analysis](Detailed%20Analysis.png)

## Project Overview

A wellness organization needs to understand how body metrics—height, weight, and BMI—vary across gender and age demographics. This understanding is critical for designing targeted fitness programs and flagging high-risk population segments. This project provides a dynamic solution through an interactive Power BI dashboard that enables deep-dive analysis of these health metrics.

## Key Insights

- **Females have consistently higher BMI** than males across every age group (25.89 vs 23.61 overall).
- **60+ females show the highest BMI** at 26.03, representing the peak risk segment in the dataset.
- **30–44 males have the lowest BMI** at 23.48, representing the fittest demographic group.
- **Overall average BMI is 24.75**, which falls within the healthy Normal range (18.5–24.9).
- **Only 21 individuals** (< 0.2% of 10,000) exceed the high BMI threshold of 36.50.

## Tools Used

- **Power BI Desktop:** Report building, data visualization, and layout design.
- **Power Query (M):** Data cleaning and feature engineering.
- **DAX:** Dynamic measure creation and threshold flagging.

## Workflow

1. **Data Loading:** Imported the 10,000-record `Gender_Classification_Data.csv` dataset.
2. **Data Transformation (Power Query):**
   - Renamed columns for readability.
   - Calculated **BMI**: `Weight / (Height/100)²`.
   - Created **Age Group** buckets (18–29, 30–44, 45–59, 60+).
   - Classified **BMI Category** (Normal, Overweight, Obese).
3. **Measure Creation (DAX):** Developed dynamic measures including Avg BMI, Total People, Avg BMI by Gender, and High BMI Count based on a 36.50 threshold.
4. **Dashboard Development - Overview Page:** Built KPIs, clustered bar charts, scatter plots, donut charts, and matrix tables linked with a cross-filtering gender slicer.
5. **Dashboard Development - Deep Dive Page:** Constructed stacked bar charts, trend lines by age/gender, and histograms to flag high-risk demographic segments.

## How to Run

1. Ensure you have **Power BI Desktop** installed on your machine.
2. Download the `Health Analytics Dashboard - Power BI.pbit` (template) and `Gender_Classification_Data.csv` files.
3. Open the `.pbit` file in Power BI Desktop.
4. When prompted, provide the local file path to the downloaded CSV dataset to load the data and view the full dashboard.

Alternatively, you can open the `.pbix` file directly if you prefer not to use the template.

## Repository Files

| File | Description |
|---|---|
| `Health Analytics Dashboard - Power BI.pbix` | Power BI project file — contains full data, visuals, and DAX measures |
| `Health Analytics Dashboard - Power BI.pbit` | Power BI template — open with the CSV to load full dashboard |
| `Gender_Classification_Data.csv` | Source dataset (10,000 records) |
| `Health Overview.png` | Dashboard Page 1 preview |
| `Detailed Analysis.png` | Dashboard Page 2 preview |

## Credits

Dataset provided by [Sameh Raouf on Kaggle](https://www.kaggle.com/datasets/samehraouf/gender-classification-dataset).
