# Global Housing Market Sensitivity Analysis (2010-2025)

## Project Overview:
This project looks into the relationship between **Real Interest Rates** and **Real House Price Index (HPI) Growth** across a global dataset. 
The study explores how the relationship between interest rates and housing prices shifted through the Pre-Pandemic, Deep Pandemic, and Recovery time periods.

## Hypotheses:
* **Hypothesis 1 ($H_1$):** There is a negative correlation between real interest rates and house price growth.
    * *Result:* **Accepted Globally.** The study identified three distinct phases: a weak pre-pandemic sensitivity, a hyper-sensitive pandemic shock, and a current normalization phase (Slope: -0.231).
* **Hypothesis 2 ($H_2$):** Developed markets are more sensitive to interest rate changes than developing markets.
    * *Result:* **Rejected.** The data revealed that Developing markets are significantly more reactive (Slope: -0.456) compared to Developed markets (Slope: -0.011), primarily due to differences in mortgage structures (Variable vs. Fixed rates).

## Methodology & Data
The project follows these steps:
1.  **Data Acquisition:** Consolidated three independent data sources from the **Bank for International Settlements (BIS)**:
    * Real Residential Property Prices
    * Central Bank Policy Rates
    * Consumer Price Index (CPI)
2.  **Feature Engineering:** * Converted Nominal Rates to **Real Interest Rates** using the Fisher Equation ($Real = Nominal - Inflation$).
    * Standardized time-series frequencies from monthly to quarterly.
3.  **Statistical Analysis:** * Ordinary Least Squares (OLS) Regression.
    * Pearson Correlation and P-value significance testing.
    * Structural Break Analysis across three distinct time "Eras."

## Visualizations
The project uses `Seaborn` and `Matplotlib` to visualize:
* The global HPI growth trends.
* Regression slopes for different economic groups and time periods.
* To compare the sensitivity between Developed and Developing economies

##  How to Run
1.  You must have Python v.3.8+ installed.
2.  Install folder: [Google Drive folder - Data Science: Housing Project (Март 2026)](https://drive.google.com/drive/folders/1-b3SyHcprsfVOlxq0zvNDoo5awYRsDSs?usp=drive_link)
   If for some reason there is a problem with opening the link, I have left the folder in github
4.  Install required libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn scipy
    ```
5.  Open `Project_housing_2.ipynb` in Jupyter Notebook or VS Code.
6.  Run all cells to replicate the analysis.

##  Project Structure
* `Project_housing_2.ipynb`: The analysis notebook containing code, math, and commentary.
* `README.md`: Project documentation and summary.
* `data/`: Directory containing raw datasets.

##  Context
Final Exam Project for the SoftUni Data Science Course (March 2026).
