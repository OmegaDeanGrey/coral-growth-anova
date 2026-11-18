# Coral Growth Analysis Using ANOVA

## Project Overview

This project examines growth differences among six genotypes of staghorn coral (*Acropora cervicornis*) to identify promising candidates for marine reef restoration.

Using Python and statistical inference, I analyzed coral growth measurements collected over one year to determine whether genotype is associated with significant differences in average linear extension.

This project was completed as part of my statistical analysis coursework.

## Research Question

Do the six coral genotypes demonstrate statistically significant differences in mean growth?

**Null Hypothesis (H₀):** All six genotypes have equal population mean growth.

**Alternative Hypothesis (H₁):** At least one genotype has a different population mean growth.

## Technologies Used

- Python
- Pandas and NumPy
- SciPy
- Matplotlib and Seaborn
- Jupyter Notebook

## Dataset

The dataset, `coral_growth.csv`, contains 3,000 growth observations across six coral genotypes, with 500 observations per genotype.

Growth is measured in centimeters of linear extension over one year.

### Descriptive Statistics

| Genotype | Mean Growth (cm) | Standard Deviation |
|---|---:|---:|
| G1 | 2.503 | 0.393 |
| G2 | 2.713 | 0.391 |
| G3 | 3.043 | 0.404 |
| G4 | 2.913 | 0.394 |
| G5 | 2.395 | 0.384 |
| G6 | 3.209 | 0.403 |

## Statistical Methodology

1. **Exploratory Data Analysis:** Calculated group means, standard deviations, and observation counts using Pandas.
2. **Visualization:** Created a Seaborn boxplot to compare growth distributions.
3. **Assumption Testing:** Used Shapiro-Wilk tests to evaluate normality and Levene's test to evaluate equality of variances.
4. **One-Way ANOVA:** Tested whether mean growth differs across the six genotypes.
5. **Tukey's HSD:** Conducted post-hoc comparisons to identify significant differences between genotype pairs.
6. **Effect Size:** Calculated eta-squared to estimate the proportion of observed growth variation associated with genotype.

## Results

The assumption checks found no statistically significant departures from normality or equality of variances at the 0.05 significance level.

The one-way ANOVA produced:

- **F-statistic:** 320.3121
- **P-value:** < 0.0001
- **Eta-squared (η²):** 0.3485
- **Variance explained:** Approximately 34.9%

These results indicate statistically significant differences in mean growth among the