# Global Housing Market Sensitivity Analysis (2010-2025)

## Project Overview:
This project looks into the relationship between **Real Interest Rates** and **Real House Price Index (HPI) Growth** across a global dataset of 36 countries. 

## Hypotheses:
* **Hypothesis 1 ($H_1$):** There is a significant inverse relationship where higher rates lead to lower price growth.
    * *Result:* **Accepted Globally.** The analysis did confirm a that as real interest rates rise, housing prices growth slows down. However, the analysis found a lag in reaction. Developed markets showed a 3-quarter lag, while developing markets reacted most in less than a quarter time.

* **Hypothesis 2 ($H_2$):** Developed markets are more sensitive to interest rate changes than developing markets.
    * *Result:* **Rejected.** The data revealed that Developing markets are significantly more reactive compared to Developed markets. The analysis found that developing markets have a strong negative reaction, while developed ones have a buffer that allows them to maintain growth. 

## Methodology & Data
The project follows these steps:
1.  **Data Acquisition:** Consolidated three independent data sources from the **Bank for International Settlements (BIS) and The Organisation for Economic Co-operation and Development(OECD)**:
    * Real Residential Property Prices -BIS
    * Central Bank Policy Rates - BIS
    * Consumer Price Index (CPI) - BIS
    * Real GDP Growth - OECD
    *  Monthly Unemployment Rates - OECD
2.  **Feature Engineering:** * Converted Nominal Rates to **Real Interest Rates** using the Fisher Equation ($Real = Nominal - Inflation$).
   * Standardized time-series frequencies from monthly to quarterly.
4. Implemented lag models to account for different market reactions.
5.   **Statistical Analysis:** * Ordinary Least Squares (OLS) Regression with interaction terms to isolate the impact of the effect while taking into consideration GDP growth and unemployment.

##  How to Run
1.  You must have Python v.3.8+ installed.
2.  Install folder: [Google Drive folder - Data Science: Housing Project (Март 2026)](https://drive.google.com/drive/folders/1-b3SyHcprsfVOlxq0zvNDoo5awYRsDSs?usp=drive_link)
3.    Install required libraries:
    ```pip install pandas numpy matplotlib seaborn statsmodels scipy ```
4.  Open `Retake_project_notebooks` in Jupyter Notebook or VS Code.
5.  Run Data_prep to see the process of cleaning the data and then open Project_analysis to view the analysis.
6.  Run all cells to replicate the analysis.

##  Project Structure
* Folder `Retake_project_notebooks`: Folder that cointains the retake version of the previous project; consists of 2 notebooks - `Data_prep.ipynb` & `Project_analysis.ipynb`
* Folder `old_project`: The originally submitted analysis notebook containing code, math, and commentary.
* `README.md`: Project documentation and summary.
* `raw_data`: Directory containing raw datasets.

##  Context
Final Exam Project for the SoftUni Data Science Course (March 2026) & Final Retake Project for the SoftUni Data Science Course (March 2026)
## Contact
For any issues with opening the drive or running the project contact me : siyanaveleva19@gmail.com 
