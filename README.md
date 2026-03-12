## Lab Activity 4.4 — Compare the Average Yields of a Specific Crop Across Multiple States
Objective
To develop and test null and alternative hypotheses to examine whether there are statistically significant differences in crop yields (e.g., Rice) across multiple Indian states using the ANOVA test.

Dataset
Agricultural Crop Yield in Indian States Dataset from Kaggle:
🔗 Kaggle Dataset Link

Requirements

Computer with Python and Jupyter Notebook installed
Python Libraries: pandas, numpy, matplotlib, seaborn, scipy, statsmodels


Prerequisites

Basic Python programming knowledge
Understanding of statistics, especially hypothesis testing
Familiarity with pandas for data manipulation
Understanding of data visualization using matplotlib and seaborn


Problem Statement
Compare the average yields of a specific crop (e.g., Rice) across multiple Indian states to determine if the differences in crop yield are statistically significant.

Steps
StepTask1Import required libraries (pandas, numpy, seaborn, matplotlib, scipy)2Load the dataset (crop_yield.csv)3Display first few rows using df.head()4Remove missing values using dropna()5Filter dataset for a specific crop (e.g., Rice)6Group yield data by state7Perform One-Way ANOVA test (f_oneway) across all state groups8Visualize yield distribution across states using a boxplot9Interpret results based on p-value

Hypothesis
HypothesisStatementH₀ (Null)No significant difference in crop yield across statesH₁ (Alternate)At least one state has a significantly different crop yield

Key Concept — ANOVA (Analysis of Variance)
ANOVA is used when comparing more than two groups at the same time. Unlike a T-Test (which compares only 2 groups), ANOVA tests whether the means of multiple groups are significantly different.
ResultConclusionp-value < 0.05Reject H₀ — significant difference in crop yield across statesp-value ≥ 0.05Fail to reject H₀ — no significant difference found

Visualization

Boxplot — Crop yield (Yield) distribution across all states (State) to visually compare yield variations


Tech Stack
LibraryUsagepandasData loading and manipulationnumpyNumerical operationsmatplotlibPlottingseabornBoxplot visualizationscipyOne-Way ANOVA test (f_oneway)statsmodelsAdditional statistical support

File Structure
Lab4_4/
├── Lab4_4.ipynb        # Main notebook
├── crop_yield.csv      # Dataset
└── README.md           # This file

Conclusion
The ANOVA test determines whether rice yield differs significantly across Indian states. A p-value below 0.05 confirms statistically significant differences, while the boxplot visually highlights which states have higher or lower yields. This analysis supports agricultural policymakers in identifying high-performing and underperforming regions for better resource allocation and crop planning.
