# Manchester-Energy-Efficiency-Insights-Dashboard
This project analyzes Energy Performance Certificate (EPC) data for Manchester (2014–2024) to uncover patterns and insights into energy efficiency, CO₂ emissions, and energy cost distribution.
The analysis integrates SQL Server for data storage and cleaning, and Power BI for data visualization, providing an interactive dashboard to support climate action and energy policy decisions.
Objectives

Analyze EPC data to identify trends in energy efficiency across property types.

Develop a Power BI dashboard integrating data from SQL Server.

Evaluate CO₂ emissions, cost distribution, and improvement potential for sustainable planning.

 Dataset

Source: EPC Open Data Communities (UK)

Dataset: Manchester EPC (2014–2024)

Key Attributes:

Property type (House, Flat, Bungalow, Maisonette)

Energy efficiency rating

CO₂ emissions

Energy consumption & cost

Potential improvement metrics

 Methodology
 Data Import

Downloaded dataset from EPC Open Data Communities.

Removed unnecessary text columns for smoother SQL import.

 Database Setup (SQL Server)

Created database: energy

Imported flat file (Manchester.csv)

Cleaned data using T-SQL:

Dropped irrelevant columns

Replaced "NO DATA" with NULL

Removed rows containing null values

 Power BI Integration

Imported cleaned dataset using:

Get Data → SQL Server → energy database

Applied data modeling and DAX calculations for key measures.

 Dashboard Visualizations
 1. CO₂ vs Efficiency Density View

Bubble chart showing the inverse relationship between CO₂ emissions and energy efficiency.

Flats and maisonettes perform best; detached houses show higher emissions.

2. Cost Distribution

Stacked bar chart of lighting, heating, and hot water costs.

Houses have the highest total energy cost (~Rs. 15M).

 3. Efficiency Improvement Potential

Lollipop chart showing potential efficiency gains by property type.

Houses (29.2%) show the highest potential improvement.

 4. Energy Flow Overview

Sankey diagram visualizing energy movement between property type, built form, and rating.

Houses and mid-terrace buildings have the highest total flow (15.4K).

 5. Current vs Potential Comparison

Comparison of current vs potential efficiency, consumption, and CO₂ emissions.

All property types show improved efficiency and lower consumption potential.

 6. Efficiency Target Tracking

Gauge chart tracking 20% efficiency improvement target.

Monitors current vs goal progress.

 7. Card Visuals

Average Energy Cost Saving: Displays potential cost reduction if optimal efficiency achieved.

CO₂ Reduction Potential: Shows total possible reduction if all properties reach target efficiency.

 Tools & Technologies
Tool	Purpose
SQL Server	Data import, cleaning, and transformation
T-SQL	Null handling and column filtering
Power BI	Dashboard creation and visualization
DAX	Calculated fields (efficiency %, CO₂ reduction, cost savings)

 Key Insights

✅ Improving energy efficiency reduces CO₂ emissions and costs simultaneously.
✅ Houses show the highest efficiency improvement potential.
✅ Heating is the largest cost driver across all property types.
✅ Visual analytics empower data-driven decisions for sustainable housing strategies.

 Conclusion

The dashboard demonstrates how SQL + Power BI integration can deliver actionable sustainability insights.
Findings reveal that high-efficiency properties have lower emissions and costs, while houses present the greatest potential for improvement.

The project supports Manchester’s goal of achieving carbon reduction and energy-efficient housing, guiding policymakers and stakeholders toward data-driven sustainability planning.

🔗 Reference

EPC Open Data Communities – Domestic Energy Performance Certificates
