# Comic Character Survival Analysis

This project investigates whether a comic book character’s identity status (e.g., Secret or Public) is associated with their likelihood of being alive, using statistical methods in R. The analysis is based on over 21,000 characters from Marvel and DC comics.

## Research Question
Is there a relationship between a character's identity status and their survival (alive or dead)?

## Methods

### Data
- Source: `comic_characters.csv` (21,144 entries)
- Key Variables:
  - `Identity`: Secret, Public, Known to Authorities, etc.
  - `Alive`: Yes or No

### Statistical Analysis
1. **Chi-Square Test of Independence**
   - Test statistic: χ² = 11.99, df = 4
   - p-value = 0.017

2. **Permutation Test**
   - 2,000 resamples
   - Empirical p-value = 0.022

## Results
Both tests indicate a statistically significant relationship (p < 0.05) between identity status and survival:
- Characters with secret identities tend to show different survival rates compared to those with public identities.
- Chi-square and permutation test results are consistent.

## How to Reproduce

### Requirements
- R (version 4.0 or higher)
- R packages: `dplyr`, `ggplot2`, `knitr`

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/comic-survival-analysis.git
