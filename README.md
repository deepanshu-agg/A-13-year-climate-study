

# A 13-Year Climate Study of Chicago and Miami

Welcome to the **A-13-year-climate-study** repository! This project investigates the impacts of climate change over 13 years in two distinct urban environments: **Chicago** and **Miami**. It provides an in-depth analysis of multiple climate parameters—ranging from temperature and UV radiation to wind speeds and precipitation patterns—to reveal trends, correlations, and insights useful for urban planning, policy-making, and further research.

---

## 1. Project Overview

### Background

- Climate change poses multifaceted challenges to urban environments, affecting temperature, humidity, precipitation, wind, and solar irradiance patterns.
- **Chicago** and **Miami** present starkly different geographies and climates, offering an excellent comparative framework to understand how climate change manifests in varied urban settings.
- This repository delves into **13 years** (2010–2022) of climate data for both cities. Through advanced data analysis techniques—such as rolling cross-correlation, fuzzy clustering, and distributional studies—this project uncovers seasonal patterns, anomalies, and potential climate-related shifts.

### Objectives

1. **Evaluative Comparison**  
   Compare key parameters (temperature, UV index, precipitation, wind speed, etc.) between Chicago and Miami to identify similarities, differences, and possible interrelations.

2. **Pattern Identification**  
   Employ robust data analysis methods (e.g., rolling cross-correlations, clustering, time-series visualizations) to detect significant trends or anomalies in each city’s climate profile.

3. **Informed Decision-Making**  
   Provide insights that can guide urban planning, policymaking, and climate adaptation strategies in both Chicago and Miami.

---

## 2. Data Sources and Parameters

The data originates from the [NASA POWER Data Access Viewer](https://power.larc.nasa.gov/data-access-viewer/). Key parameters include:

- **ALLSKY_SFC_UV_INDEX, ALLSKY_SFC_UVB, ALLSKY_SFC_UVA**: Surface UV measurements.  
- **TS**: Earth Skin Temperature (land surface temperature).  
- **T2M**: Air Temperature at 2 meters above ground.  
- **T2MDEW**: Dew/Frost Point at 2 meters.  
- **T2M_RANGE**: Range of temperatures at 2 meters.  
- **PRECTOTCORR**: Corrected Total Precipitation.  
- **QV2M**: Specific Humidity at 2 meters.  
- **PS**: Surface Pressure.  
- **WS10M_RANGE, WS2M, WS2M_RANGE**: Wind Speed measurements at various heights and ranges.

Please see the `dataset_parameters_description.pdf` in this repository for further details on each parameter.

---

## 3. Methodology

### 3.1 Data Preparation
- **Data Cleaning**: Handling missing or anomalous values, ensuring time alignment for multi-year comparisons.  
- **Parameter Selection**: Focus on temperature (TS, T2M, T2M_RANGE), UV radiation (UVB, UVA, UV Index), humidity (QV2M, T2MDEW), precipitation (PRECTOTCORR), and wind (WS2M, WS10M_RANGE).

### 3.2 Rolling Cross-Correlation
- **Goal**: Examine how correlations between parameters evolve over time (e.g., every 2-month window).  
- **Outcome**: Heatmaps and distance matrices highlight periods of strong/weak correlations and detect potential seasonal shifts or anomalies.

### 3.3 Clustering (Fuzzy C-Means)
- **Goal**: Identify groupings within the data based on similarity of parameters.  
- **Outcome**: Density heatmaps and cluster labels show how UV radiation, temperature, and other parameters group together or deviate across seasons and years.

### 3.4 Distribution & Time-Series Analysis
- **Density Plots**: Display the distribution of parameters (e.g., UVB) by year, capturing changes or anomalies.  
- **Time-Series Plots**: Visualize trends, spikes, or dips in climatic variables over the 13-year span.

### 3.5 Statistical Testing
- **Z-Tests / Standard Deviation Plots**: Assess variations from mean values across different years, indicating potential shifts in baseline climate conditions.

---

## 4. Key Findings

1. **Temperature-UV Relationship**  
   - Both cities show a strong correlation between rising surface temperatures and UV intensity, though seasonal variations differ significantly (more pronounced summer peaks in Miami).

2. **Precipitation Variability**  
   - Chicago’s precipitation patterns show more noticeable peaks in certain years compared to Miami. Rolling correlation analyses suggest potential shifts in seasonal precipitation timing.

3. **Wind Speed & Humidity**  
   - Wind speed fluctuations correlate with humidity changes, but the magnitude differs between cities, possibly due to geographic and coastal factors in Miami versus inland patterns in Chicago.

4. **Temporal Shifts**  
   - Distance matrices of rolling cross-correlation indicate that some climate parameter relationships have evolved notably over the 13-year period, highlighting potential early signals of ongoing climate shifts.

For a deeper dive into the methodology, visualizations, and interpretations, refer to the **Climate change project_Report.pdf** included in this repository.

---

## 5. Future Outlook

- **Expanded Parameter Set**: Incorporate additional factors such as air quality indices or oceanographic data (for Miami) to gain a more holistic climate picture.  
- **Longer Time Horizon**: Extending the analysis beyond 13 years may confirm whether detected trends are persistent or cyclical anomalies.  
- **Predictive Modeling**: Use machine learning models (e.g., LSTM networks) to forecast future climate patterns and inform proactive urban planning.  
- **Comparative Urban Studies**: Apply this framework to other major cities, creating a broader comparative map of climate change impacts across diverse geographies.

---

## 6. Repository Structure

Below is an overview of the key files and folders in this repository:

```
A-13-year-climate-study/
├── Code_Notebooks/
│   ├── Prj_CHICAGO.ipynb
│   │     (Notebook with core analysis for Chicago's data)
│   ├── Prj_MIAMI.ipynb
│   │     (Notebook with core analysis for Miami's data)
│   ├── Rolling_cross_matrix_Chicago.ipynb
│   │     (Rolling cross-correlation analysis for Chicago)
│   └── Rolling_cross_matrix_Miami.ipynb
│         (Rolling cross-correlation analysis for Miami)
├── dataset_CHICAGO.csv
│     (Raw climate data for Chicago)
├── dataset_MIAMI.csv
│     (Raw climate data for Miami)
├── dataset_parameters_description.pdf
│     (Detailed descriptions of each climate parameter)
├── Climate change project_Report.pdf
│     (Full project report with methodology, figures, and discussion)
└── README.md
      (This README file)
```

---

## 7. References

1. **Data Source**:  
   - [NASA POWER Data Access Viewer](https://power.larc.nasa.gov/data-access-viewer/)  
2. **Literature**:  
   - Orte, F. et al. *Comparison of NASA-POWER solar radiation data with ground-based measurements in the south of South America.* IEEE, 2021.  
   - White, J.W. et al. *Evaluation of satellite-based, modeled-derived daily solar radiation data for the continental United States.* *Agronomy Journal*, 2011.  
   - Chandler, W.S. et al. *Near real-time global radiation and meteorology web services available from NASA.* *Solar 2010 Conference*, 2010.

For more detailed references and discussions, please see the **Climate change project_Report.pdf** included in this repository.

---

### Disclaimer
This project is for educational and research purposes. The data, findings, and interpretations are provided “as-is” and do not constitute official advice for policy or urban planning without further peer review and validation.

---

Thank you for exploring this repository! We hope the analyses, visualizations, and insights here spark further research and informed actions around urban climate adaptation and sustainability. Feel free to explore each notebook, review the data, and consult the full PDF report for an in-depth narrative of our 13-year climate study on Chicago and Miami.
