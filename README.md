# Aircraft Risk Analysis – Phase 1 Data Science Project

## Project Overview
This project analyzes aircraft accident data to assist a company expanding into the aviation sector in selecting safer aircraft models for commercial and private operations.  
The analysis focuses on identifying aircraft models with the lowest fatality rates and summarizing broader manufacturer trends.

## Business Problem
The company seeks to diversify into aviation but lacks sufficient insights into aircraft risk profiles.  
Using historical accident and fatality data, this project provides data-driven recommendations to help select lower-risk aircraft models for acquisition.

## Data
- Source: National Transportation Safety Board (NTSB) dataset.
- Key Columns:
  - `Model`: Specific aircraft model (e.g., 172N, PA-28-140).
  - `Make`: Manufacturer name (e.g., Cessna, Piper).
  - `Total.Fatal.Injuries`: Number of fatalities recorded per event.
  - `Event.Id`: Unique identifier for each accident/incident.

## Key Analysis Steps
- Standardized manufacturer names by cleaning casing inconsistencies in the `Make` column.
- Grouped data by `Model` to compute:
  - Total accidents.
  - Total fatalities.
  - Fatality rates (fatalities divided by accidents).
- Filtered out aircraft models with fewer than 30 recorded accidents for meaningful statistical reliability.
- Identified:
  - Top 10 safest aircraft models (lowest fatality rates).
  - Top 10 riskiest aircraft models (highest fatality rates).

## Results Summary
- **Most Common Aircraft Models**: Cessna 152, Cessna 172, Piper PA-28-140.
- **Safest Models**: Small general aviation planes like the Cessna 172 showed the lowest fatality rates.
- **Riskier Models**: Older large commercial jets such as the Boeing 747-168 and Tupolev TU-154 had the highest fatality rates per accident.

## 📊 Interactive Tableau Dashboard

Explore the full dashboard here:  
 [View on Tableau Public](https://public.tableau.com/app/profile/anthony.njiru/viz/Phase1_Aviation_Dashboard/AviationRiskAnalysisDashboard?publish=yes)

This dashboard allows stakeholders to:
- Filter by aircraft make/model
- Explore accident trends by year
- View fatality rates by phase of flight

<div style="background-color:rgb(81, 133, 139); border: 2px solid #ccc; border-radius: 8px; padding: 16px;">

| **Final Business Recommendations** |   |
|:----------------------------------:|:-:|
| **1. Acquire Cessna 172 Skyhawk**<br>*(Make: Cessna)* | Why: This model has the largest sample size (2,200+ accidents) and one of the lowest mean fatality rates (~0.035 fatalities per accident). Its ubiquity ensures the metric is statistically robust. |
| **2. Acquire Piper PA-28 Cherokee Variants**<br>*(Make: Piper)* | **Models:** PA-28-140 Cherokee Cruiser and PA-28-180 Cherokee.<br>**Why:** Each has over 900 recorded incidents with mean fatality rates below 0.05. They’re proven workhorses in both training and private operations. |
| **3. Build a Diversified Fleet & Enhance Safety Protocols** | **Fleet Mix Proposal:**<br>- 50% Cessna 172 Skyhawks<br>- 25% Cessna 182 Skylanes (Make: Cessna)<br>- 25% Piper PA-28-180 Cherokees |

</div>

## 📂 Quick Access to Key Files

- 📓 [Final Jupyter Notebook (`phase1_project.ipynb`)](https://github.com/TonieMuthee/phase_1_data_science_project/blob/main/Notebook_phase1_project.ipynb)
- 📄 [Notebook PDF Export (`phase1_project.pdf`)](notebooks/phase1_project.pdf)
- 🎥 [Non-Technical Presentation (`presentation.pdf`)](https://github.com/TonieMuthee/phase_1_data_science_project/blob/main/Presentation_Identifying_Lowest_Risk_Aircraft_for_Investment.pdf)
- 📊 [Tableau Dashboard (Interactive)](https://public.tableau.com/app/profile/anthony.njiru/viz/Phase1_Aviation_Dashboard/AviationRiskAnalysisDashboard?publish=yes)

## How to Run
1. Clone this repository.
2. Install requirements:  
