# Prince George's County Crime Analysis (2025)
<img width="250" height="323" alt="Seal_of_Prince_George's_County,_Maryland_(1958–1971) svg" src="https://github.com/user-attachments/assets/3f4a6f34-380e-4f5c-8833-fcb2618ef129" />

This project analyzes crime incidents in Prince George's County, Maryland for the year 2025. The goal is to identify the most frequent types of crime and visualize where these crimes occur.

## Overview of the Code

1. **Data Loading and Filtering**
   - The dataset is a CSV file of crime incidents from Prince George's County. 
  You can download it manually from the county’s [Open Data Portal](https://data.princegeorgescountymd.gov/) by searching for "Crime Incidents" or the dataset for 2023–present.
   - Loaded into Python using **Pandas**.
   - Filtered to include only crimes from 2025.

2. **Data Cleaning**
   - Removed unnecessary columns: `PGPD Reporting Area`, `PGPD Sector`, `PGPD BEAT`, `Street Number`, `Street Name`.
   - Ensured no null values in relevant columns: `Date`, `Clearance Code`, `Latitude`, `Longitude`.

3. **Exploratory Data Analysis (EDA)**
   - Counted the number of occurrences for each crime type.
   - Created a **bar chart** showing the top 10 most frequent crimes in 2025 using **Matplotlib**.

4. **Spatial Visualization**
   - Used the **Folium** library to create a **HeatMap** of crime locations across the county.
   - Zoomed in on the **University of Maryland campus** to observe localized crime hotspots.

## Key Libraries
- `pandas` – Data manipulation and filtering.
- `matplotlib` – Visualization of top crimes with bar charts.
- `folium` – Interactive maps and HeatMap visualizations.

## Usage
1. Place the CSV file in the project directory.
2. Run the Python script (e.g., `crime_analysis.py`).
3. The script outputs:
   - Bar chart of top 10 crimes.
   - HeatMap HTML files showing spatial distribution of crimes.

## Limitations
- Only includes reported crimes for 2025; unreported crimes are not captured.
- City-level data is missing; latitude/longitude is used instead.
- Analysis reflects only short-term trends.

## Author
**Wuilmer Palacios**
