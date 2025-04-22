# Comic Character Survival Analysis

This project explores the relationship between a comic book character’s identity status and their survival (alive or dead) using statistical inference in R. The dataset contains over 21,000 Marvel and DC characters.

## Objective

To test whether a character’s identity type (e.g., Secret, Public) is statistically associated with their alive status using categorical inference methods.

## Dataset

- **Source**: `comic_characters.csv` (21,144 observations)
- **Key Variables**:
  - `Identity` — Categorical (Secret, Public, Known to Authorities, etc.)
  - `Alive` — Binary (Yes/No)

## Methods

1. **Chi-Square Test of Independence**  
   Used to assess the association between two categorical variables.
   - χ² = 11.99, df = 4, p = 0.017

2. **Permutation Test**  
   A non-parametric resampling approach (2,000 iterations) to empirically assess significance.
   - Empirical p-value = 0.022

Both tests support rejecting the null hypothesis at the 0.05 significance level.

## Results

There is a statistically significant association between a character’s identity status and their survival outcome. Characters with public and secret identities show different distributions in survival rates.

## Files

- `ChiSquare.Rmd` — Full R Markdown with code and analysis
- `ChiSquare.html` — Rendered report with visualizations
- `comic_characters.csv` — Dataset used in the analysis
