# Titanic_Dataset_PowerBI
🚢 Titanic Survival Analysis (PowerBI Project)
<img width="1162" height="663" alt="Screenshot 2025-11-07 135457" src="https://github.com/user-attachments/assets/ce3fef42-5f00-48eb-99a0-0a2f85494500" />

Overview
This repository contains an Excel Workbook dedicated to analyzing the famous Titanic Passenger Data. We use Pivot Tables, Formulas, and Slicers to explore the factors that influenced survival during the disaster, test key historical hypotheses (like "women and children first"), and uncover patterns in the passenger manifest.

💾 Data Source
The core data is the standard Titanic.xlsx file, saved as a workbook with the raw data on one sheet and the analysis/dashboard on another.

Column	Description	Key Values for Analysis
Survived	Survival Status	1 (Yes) or 0 (No)
Pclass	Passenger Class	1st, 2nd, 3rd
Sex	Gender	male, female
Age	Passenger Age	Numerical (Used for Age Grouping)
Fare	Ticket Fare	Numerical (Used for Averages)
Embarked	Port of Embarkation	C (Cherbourg), Q (Queenstown), S (Southampton)

Export to Sheets
🔑 Key Analysis Components
The Excel workbook is structured around several Pivot Tables and a final Dashboard to answer core analytical questions:

1. Core Pivot Tables
These tables form the foundation of the analysis:

Survival by Class and Gender: A Pivot Table showing the average of the Survived column (which gives the survival rate percentage) broken down by Pclass (Rows) and Sex (Columns).

Fare Analysis: A Pivot Table calculating the average Fare paid, grouped by Pclass and Survived status.

Passenger Counts: A Pivot Table counting passengers by Embarked port and Pclass.

2. Formulas & Calculated Fields
Custom Excel formulas are used to create enhanced features:

Age Group: An auxiliary column created using an IF or VLOOKUP formula to categorize Age into groups (e.g., Child, Adult, Senior) for better analysis.

Is Alone: A column created using an IF formula to check if the sum of SibSp and Parch is zero.

3. Interactive Dashboard
The dashboard sheet uses charts created from the Pivot Tables and is controlled by Slicers for easy filtering:

Slicer Controls: Pclass, Sex, Survived, and Age Group.

Visualizations: Charts illustrating survival rate distribution, average fares, and passenger demographics.

💡 Key Insights from the Data
The Excel analysis reveals several powerful and statistically significant patterns:

Gender was the Strongest Predictor: The analysis confirms the "women and children first" protocol.

Females had a survival rate approximately 4 times higher than males (around 74% vs. 19%).

Socio-economic Status was Critical: Survival rates were directly proportional to ticket class.

1st Class passengers had the highest survival rate (around 63%).

3rd Class passengers had the lowest survival rate (around 24%).

Fares and Survival: The average fare paid by those who survived was significantly higher than those who perished, particularly within 1st class, indicating a potential correlation between the price/location of the cabin and rescue priority.

Traveling Alone was a Disadvantage: Passengers traveling alone (based on the Is Alone calculated field) had a noticeably lower chance of survival compared to those who boarded with family members.

🚀 Getting Started
To explore this analysis, you only need Microsoft Excel:

Download: Clone or download the entire repository.

Open: Open the Titanic.xlsx file.

Explore: Navigate to the "Dashboard" sheet to start interacting with the Slicers and see the analysis results instantly.

Audit: Review the "PivotTables" sheet to inspect the raw data summaries used to power the dashboard charts.
