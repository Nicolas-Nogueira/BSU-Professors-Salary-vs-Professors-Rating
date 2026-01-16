Professor Salary vs Rating Analysis - Bridgewater State University

Overview
This project investigates the relationship between professor salaries and student ratings at Bridgewater State University (BSU). The analysis tests whether Rate My Professors ratings have any association with faculty base pay.

Research Question
Do professor ratings meaningfully relate to base pay (salary) at Bridgewater State University?

Hypothesis: University salary structures are primarily determined by institutional factors (rank, experience, discipline) rather than student evaluations, so we expect to find no significant relationship between ratings and salary.
Key Findings

Correlation: r = -0.074 (essentially no linear relationship)
Statistical Significance: p = 0.328 (not significant at α = 0.05)
Explanatory Power: r² = 0.0055 (only 0.55% of salary variation explained by rating)
Prediction Error: $26,640 (approximately 35% of mean salary)

Conclusion: Professor ratings show no significant relationship to salary. Compensation is driven by institutional factors like rank, experience, and discipline rather than student evaluations.
Data Sources
Professor Rating Data

Source: Rate My Professors (ratemyprof.com)
Metric: Average professor rating on a 1.0–5.0 scale
Represents: Student perceptions of teaching quality and experience

Salary Data

Source: Massachusetts State Payroll website (cthrupayroll.mass.gov)
Year: 2025
Institution: Bridgewater State University
Filter: Full-time employees with "Professor" title only

Dataset Structure
Sample Size: 175 professors
Variables:

Employees: Professor name
Base Pay: Annual salary ($)
dept: Academic department
rating: Average Rate My Professors rating

Summary Statistics:

Salary: Mean = $77,097, SD = $26,641, Range = $3,445 - $120,794
Rating: Mean = 3.69, SD = 0.74, Range = 1.7 - 5.0

Project Files
.
├── BSU_prof_salary.csv          # Raw dataset
├── BSU Prof Salary vs Prof Rating.Rmd  # R analysis notebook
├── dashboard.html               # visualization dashboard
└── README.md                    # This file

Analysis Methods

Exploratory Data Analysis

Summary statistics
Scatterplot visualization


Correlation Analysis

Pearson correlation coefficient
Coefficient of determination (r²)


Linear Regression

Least-squares regression: ŷ = 87,024 - 2,687x
Residual analysis
Hypothesis testing


Interactive Dashboard

Salary vs rating scatter plot
Department-level comparisons
Distribution visualizations



How to Use
R Markdown Analysis

Open BSU Prof Salary vs Prof Rating.Rmd in RStudio
Ensure the CSV file is in the same directory
Run all chunks to reproduce the analysis

Interactive Dashboard

Open dashboard.html in any modern web browser
Explore interactive visualizations
Hover over data points for detailed information

Technical Requirements
R Analysis:

R (version 3.5+)
No additional packages required (uses base R)

Dashboard:

Modern web browser with JavaScript enabled
No installation required (uses CDN-hosted Vega libraries)

Interpretation
The negligible correlation and lack of statistical significance confirm that professor salaries at BSU are determined by:

Academic rank
Years of experience
Discipline/field
Administrative responsibilities
Collective bargaining agreements

Student ratings, while potentially valuable for formative feedback, do not function as a merit-based pay mechanism in this institutional context.
Limitations

Cross-sectional data (single time point)
Matching is limited to professors appearing in both datasets
Does not control for confounding variables (rank, years of service, etc.)
Some low salary values may reflect part-time or temporary appointments

Future Directions
Future research could examine:

Direct effects of rank, years since PhD, and discipline on salary
Longitudinal analysis of salary progression
Comparison across multiple institutions
Impact of administrative roles and grant funding
