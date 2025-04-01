# Project-Genetic-Marker-HeartAttacks

## Disclaimer:
This project uses **simulated data** for educational purposes only. No real human genetic data is included. 

**Executive Summary: Identifying Genetic Marker for Sudden Heart Attacks**
By Krishna Priya Nemalikanti

**Obejctive:**
This project aims to identify potential genetic marker associated with sudden heart attacks using a simulated dataset.The goal was to demonstrate a beginner-friendly data science workflow for genetic association studies, covering topics like data exploration, statistical testing, multiple testing correction and visualization.

**Key Genetic terms used in the Project:**
SNP : Single Nuclotide Polymorphism. A single DNA change. These are the "data points" in genetic studies.
Allele : Variant of a SNP
Odds Ratio (OR) : Measures how much an allele increases risk
95% CI : Confidence Interval for the Odds Ratio
GWAS : Genome-wise association study.

**Approach:**
1.Data Simulation
Generated a dataset of 1000 individuals (500 cases with heart attacks and 500 controls)
Simulated 50 genetic markers (SNPs) with 5 designed to have a true association with heart attacks.

2.Quality Control
Checked for missing data
Visualized allele frequency distribution to ensure data integrity.

3.Statistical Analysis
Performed chi-square tests to assess association between SNPs and heart attach risk
Calculated odds ratio (OR) to measure the effect sizes.
OR = 1 No effect (SNP doesn't influence risk)
OR > 1 SNP increases heart attack risk ( OR=2 means twice as likely to have a heart attack if the risk allele is present)
OR < 1 SNP may be protective, indicative of reduces risk

4.Mutlitple Testing Correlation
Applied Bonferroni correction to control for false positives due to testing multiple SNPs.

5.Visualization & Interpretation
Created a Manhattan plot to highlight significant SNPs
Plotted odds rations for the most promising genetic markers

**Key Findings:**
Successfulyy identified simulated risk SNPs (SNP_45 to SNP_49) with statistically significant association (p-value < 0.05 after correction).
The strongest associations had odds ratios > 1.5, indicating increased heart attack risk.
Demostrated that proper multiple correction is essential to avoid false positive discoveries.

**Significance & Applications:**
This project provides a foundational framework for genetic association studies
Can be extended to real-worl datasets (e.g., genome-wide association studies, or GWAS)
Potential application in precision medicine for early risk prediction and personalized treatment.

**Limitations & Future work possibilities:**
Used simulated data, real genetic datasets are more complex
Simplified statistical methods (chi-square instead of regression)
Future improvements could include:
Incorporating covariates (age, sex, lifestyle factors)
Using Machine Learning for risk scoring
Applying more advanced multiple testing methodologies like false discovery rate control.

**Conclusion:**
This project successfully demostrated a basic genetic association study workflow, identifying simulated risk markers for sudden heart attacks. While simplied, it can serve as an educational foundation for more advanced bioinformatics applications.
