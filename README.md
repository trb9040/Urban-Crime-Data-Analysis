# Urban Crime Data Analysis: District, Temporal & Arrest Patterns

**Northeastern University | IE 6400: Foundations for Data Analytics Engineering | Fall 2026**

## Project Overview

This project analyzes 28,100 instructional urban crime incident records from 2020–2024 to investigate geographic patterns, temporal trends, and arrest outcomes.

Working collaboratively in a three-member graduate research team, we developed a complete data analytics workflow involving data cleaning, exploratory data analysis (EDA), statistical hypothesis testing, visualization, and validation.

The objective was to transform an inconsistent dataset into reliable analytical results and communicate meaningful findings using Python and statistical methods.

## Tools & Technologies

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib
- **Statistical Analysis:** SciPy
- **Development Environment:** Jupyter Notebook
- **Methods:** Chi-square tests, permutation tests, confidence intervals, descriptive statistics, cross-tabulations

## Dataset Description

The instructional dataset contained:

- **28,100** original incident records
- **28,000** unique incidents after cleaning
- **11** original variables
- **15** variables after feature creation
- **12** police districts
- **10** standardized crime categories
- **Time Period:** January 2020 – December 2024

**Note:** This dataset was created for educational purposes and modeled on the structure of public urban crime records. It does not represent actual crime statistics for Chicago or any other city.

## Data Cleaning & Preparation

Identified and addressed seven data-quality issues:

1. Inconsistent Boolean values
2. Inconsistent crime category labels
3. Exact duplicate records
4. Hidden duplicates caused by inconsistent values
5. Invalid date entries
6. Missing and invalid geographic coordinates
7. Inconsistent location descriptions

### Cleaning Results

- Reduced the dataset from 28,100 to 28,000 unique incidents.
- Standardized categorical labels and Boolean values.
- Converted invalid dates into missing timestamps.
- Replaced invalid coordinate values with missing values.
- Created additional temporal variables for analysis.
- Verified that no duplicate incident IDs remained.

## Research Questions & Key Findings

### Research Question 1: Are Crime Types Associated with Police Districts?

**Methods Used:**
- Cross-tabulations
- Chi-square test of independence
- Cramér's V
- Permutation testing

**Results:**
- Crime-type distributions were nearly identical across all 12 districts.
- Chi-square statistic: 93.7
- p-value: 0.63
- Cramér's V: 0.019

**Conclusion:** No statistically significant association between police district and crime category was identified within the instructional dataset.

### Research Question 2: How Did Recorded Incidents Change from 2020–2024?

**Methods Used:**
- Time-series analysis
- Annual and monthly aggregations
- Descriptive statistics
- Data visualization

**Results:**
- Annual incident totals ranged from 5,549 to 5,623.
- The largest year-over-year change was a 1.32% decrease.
- Monthly incident counts ranged from 371 to 520.
- No consistent seasonal peak was identified.

**Conclusion:** Recorded incident totals remained relatively stable across the five-year period, despite monthly fluctuations.

### Research Question 3: How Do Arrest Percentages Differ Across Crime Types?

**Methods Used:**
- Categorical comparisons
- Chi-square testing
- 95% confidence intervals
- Statistical visualization

**Results:**

| Crime Type | Arrest Percentage |
|------------|------------------:|
| Narcotics | 62.0% |
| Assault | 23.1% |
| Battery | 18.4% |
| Other Offense | 14.2% |
| Robbery | 12.3% |
| Burglary | 10.4% |
| Criminal Damage | 8.4% |
| Theft | 7.4% |
| Motor Vehicle Theft | 7.1% |
| Deceptive Practice | 5.4% |

**Overall Arrest Percentage:** 13.8%

**Statistical Results:**
- Chi-square statistic: 2,958.6
- p-value: < 0.001
- Cramér's V: 0.325

**Conclusion:** Crime category demonstrated a statistically significant association with arrest outcomes. Narcotics incidents had the highest percentage of recorded arrests.

## Data Validation

To ensure reliable results, the team:

- Verified row counts and dataset dimensions after cleaning.
- Confirmed that all duplicate incidents were removed.
- Validated category counts and missing-value summaries.
- Cross-checked annual incident totals using independent calculations.
- Compared chi-square results with permutation testing.
- Evaluated limitations caused by missing data.

## Key Skills Demonstrated

- Python Programming
- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Statistical Hypothesis Testing
- Data Quality Assessment
- Data Visualization
- Analytical Problem-Solving
- Technical Communication
- Collaborative Research

## Project Files

- `IE6400_Project1_Complete.ipynb` — Complete Python analysis, statistical tests, and visualizations.
- `IE6400_Project1_Final_Report.pdf` — Collaborative graduate project report.
- `requirements.txt` — Python libraries required to run the notebook.
- `README.md` — Project overview, methodology, and key findings.

## How to Run the Project

1. Download or clone this repository.
2. Install the required Python libraries:

   ```bash
   pip install -r requirements.txt
   ```

3. Open `IE6400_Project1_Complete.ipynb` in Jupyter Notebook.
4. Place the original instructional dataset, `IE6400_Project1_UrbanCrime_Instructional.csv`, in the same working directory as the notebook.
5. Run the notebook cells in order.

**Dataset Availability:** The original instructional dataset was provided for academic coursework and is not included in this public repository. The notebook contains saved analytical results and visualizations that can be viewed without running the code.

## Project Contributors

This project was completed collaboratively as part of Northeastern University's IE 6400 Foundations for Data Analytics Engineering course.

**Team Members:**
- Tyler Brown
- Arihant Artheeswari Mugundan
- Anandi Kodali

## Future Improvements

Potential extensions of this project include:

- Exploring day-of-week and hourly incident patterns.
- Investigating relationships between incident location and arrest outcomes.
- Developing interactive dashboards and visualizations.
- Applying predictive modeling techniques to explore incident characteristics.

## Project Limitations

This analysis uses an instructional dataset rather than official police records.

Findings describe statistical patterns within the supplied dataset and should not be interpreted as real-world crime rates, policing effectiveness, or causal relationships.

---

**Academic Portfolio Project | Northeastern University | MS Data Analytics Engineering | 2026**
