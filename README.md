🌧️ Standardized Precipitation Index (SPI) — Bangladesh Rainfall Analysis

This repository contains a **demo dataset and workflow** for computing the Standardized Precipitation Index (SPI), using rainfall data from meteorological stations across Bangladesh. The project demonstrates the manual SPI computation process as well as the pre-processed data used for verification and reproducibility.

1. `Barisal_SPI_Calculation_Demo.xlsx`

A demo Excel file showing the SPI calculation workflow for Barisal station

All rainfall values (monthly dataset) are preserved.
All formulas, equations, and intermediate gamma-distribution functions were removed, leaving only the final processed values.
This file is suitable for demonstration, learning, or referencing.

2. Full Dataset (31 Stations) — Private

SPI was computed for 31 meteorological stations across Bangladesh (1989–2023)
These include major divisions and drought-prone regions such as:
* Rajshahi
* Ishwardi
* Dinajpur
* Rangpur
* Sylhet
* Dhaka
* Barisal
* Chittagong
* Khulna
* …and others

Overview of the SPI Methodology
This project follows the standard **SPI computation procedure**, including:

1. Gamma Distribution Fitting

Rainfall series → Probability distribution → Shape & scale parameters.

2. Cumulative Distribution Function (CDF)

Converted probabilities → Standardized Z-scores.

3. SPI Classification

Based on McKee et al. (1993) drought thresholds:

| SPI Value     | Category       |
| ------------- | -------------- |
| ≥ 2.0         | Extremely Wet  |
| 1.5 to 1.99   | Very Wet       |
| 1.0 to 1.49   | Moderately Wet |
| -0.99 to 0.99 | Near Normal    |
| -1.0 to -1.49 | Moderately Dry |
| -1.5 to -1.99 | Severely Dry   |
| ≤ -2.0        | Extremely Dry  |

4. Time Periods Computed

SPI-1 (Monthly)
Future extension: SPI-3 / SPI-6 / SPI-12 (Seasonal–annual scales)

Key Features of This Project

* Manual SPI computation using Excel (Gamma fitting + Z-score transformation).
* Dataset includes **31 climate stations** across Bangladesh.
* SPI helps identify:
  * Drought cycles
  * Intra-seasonal variability
  * Long-term rainfall anomalies
  * Dry-day patterns
  * Monsoon behavior shifts

This project supports drought monitoring, water resource assessment, and climate-risk studies.


Tools Used

| Tool                  | Purpose                                       |
| --------------------- | --------------------------------------------- |
| **Excel**             | Gamma distribution fitting, SPI-1 calculation |
| **Python (Optional)** | Future automation of SPI computation          |
| **ArcGIS/QGIS**       | Spatial mapping and visualization             |
| **BMD Rainfall Data** | Observed monthly rainfall (1989–2023)         |



How to Use This Repository

1. Open `Barisal_SPI_Calculation_Demo.xlsx`.
2. Review the cleaned SPI setup:
   * Rainfall values
   * Intermediate probability values (if included)
   * Final SPI outputs
3. Use the demo as a reference to compute SPI for other stations.
4. Extend with Python scripting for automation (optional).
5. Use outputs for:
   * Drought mapping
   * Research
   * Climate analysis
   * Academic reports

Future Work
* Adding **Python script** for automated SPI computation.
* Uploading **full 31-station dataset** with SPI outputs.
* Publishing spatial drought maps using ArcGIS/QGIS.
* Adding SPI-3, SPI-6, SPI-12 (seasonal & long-term scales).

---

