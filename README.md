# 🚀 Rocket Engine Performance Analysis Using Excel

## Project Overview
This project analyzes rocket engine performance data to evaluate how fuel type, oxidizer type, chamber pressure, and oxidizer–fuel ratio affect engine efficiency, stability, and physics compliance. The analysis was performed entirely in **Excel** using pivot tables and charts to generate actionable insights.

---

## Dataset
The dataset includes the following columns:

| Column | Description |
|--------|-------------|
| `fuel_type` | Type of fuel used (e.g., LH2, RP-1) |
| `oxidizer_type` | Type of oxidizer (e.g., LOX, NTO) |
| `chamber_pressure_bar` | Combustion chamber pressure in bar |
| `oxidizer_fuel_ratio` | Ratio of oxidizer to fuel |
| `combustion_temperature_K` | Combustion temperature in Kelvin |
| `heat_capacity_ratio` | Thermodynamic efficiency factor (γ) |
| `nozzle_expansion_ratio` | Nozzle efficiency factor |
| `ambient_pressure_bar` | Ambient pressure outside engine |
| `specific_impulse_s` | Engine efficiency metric (KPI) |
| `combustion_stability_margin` | Safety margin for combustion stability |
| `physics_violation_flag` | 1 = violation detected, 0 = valid |

---

## Tools & Skills
- **Excel**: Pivot tables, charts, filters 
- **Data Cleaning**: Handling missing values, duplicates, invalid entries  
- **Visualization**: Bar charts, line charts, column charts  

---

## Analysis Performed

### Data Cleaning
- Removed duplicates and invalid values (negative pressures or temperatures)  
- Verified numeric data types for all performance metrics  
- Handled missing values appropriately without biasing results  

### Pivot Tables
1. **Fuel Performance:** Average `specific_impulse_s` by fuel type  
2. **Oxidizer Impact:** Average `specific_impulse_s` and record count by oxidizer type  
3. **Pressure vs Performance:** Average `specific_impulse_s` across chamber pressure ranges  
4. **Physics Violations:** Count of violations per fuel type  
5. **O/F Ratio Analysis:** Average `specific_impulse_s` across oxidizer–fuel ratio ranges  

### Charts
- Bar chart: Average performance by fuel type  
- Column chart: Average performance by oxidizer type  
- Line chart: Chamber pressure vs average specific impulse  
- Bar chart: Physics violations count by fuel  
- Line chart: O/F ratio vs average performance  

---

## Key Insights
- Certain fuel–oxidizer combinations produce higher efficiency but with narrower stability margins.  
- Chamber pressure improves performance up to a limit, beyond which combustion stability decreases.  
- Physics violations cluster at extreme O/F ratios and high temperatures, indicating unsafe operating regions.  
- Optimal operating ranges were identified to balance performance and safety.  

---

## How to Use
1. Open the Excel file.  
2. Review `Raw_Data` for the original dataset.  
3. Check `Clean_Data` for cleaned dataset ready for analysis.  
4. Navigate to `Pivot_Analysis` to see the pivot tables and corresponding charts.  
5. Use slicers/filters to explore specific fuel or oxidizer combinations.  

---

## Resume Bullet Version
- Cleaned and validated rocket engine dataset with Excel.  
- Created pivot tables and charts to analyze relationships between fuel, oxidizer, pressure, mixture ratio, and performance.  
- Delivered actionable insights on optimal operating ranges and physics violation risks.
