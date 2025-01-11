# Hypothesis Testing in Healthcare: Drug Safety

## Project Overview

This project examines the safety profile of a new drug based on a randomized controlled trial conducted by **GlobalXYZ**, a pharmaceutical company. The focus is to assess whether the drug has any significant adverse effects compared to a placebo group. The dataset, originally from **Hbiostat** and curated by the Vanderbilt University Department of Biostatistics, has been modified for this analysis.  

The non-profit organization that commissioned this analysis is particularly interested in identifying statistically significant adverse reactions and the relationship between treatment (Drug vs. Placebo) and the number of adverse effects.

---

## Dataset Description

The modified dataset, `drug_safety.csv`, includes the following columns:

| Column            | Description                                                  |
|--------------------|--------------------------------------------------------------|
| `sex`             | The gender of the individual                                 |
| `age`             | The age of the individual                                    |
| `week`            | The week of the drug testing                                 |
| `trx`             | Treatment groups: Drug or Placebo                           |
| `wbc`             | White blood cell count                                      |
| `rbc`             | Red blood cell count                                        |
| `adverse_effects` | Indicates the presence (`Yes`/`No`) of at least one adverse effect |
| `num_effects`     | The total number of adverse effects experienced by an individual |

---

## Objectives

1. Assess whether the proportion of adverse effects differs significantly between the Drug and Placebo groups using statistical tests.
2. Investigate if the number of adverse effects (`num_effects`) is independent of the treatment group.
3. Explore demographic trends, such as age distribution, and their relationship with treatment groups.
4. Perform additional exploratory data analyses (EDA) to uncover patterns in adverse effects and demographic/vital signs data.

---

## Methods

### Statistical Analyses
1. **Two-Proportion Z-Test**:  
   Evaluate whether the proportion of individuals with adverse effects (`adverse_effects`) significantly differs between the Drug and Placebo groups.

2. **Chi-Square Test of Independence**:  
   Test the independence between the treatment group (`trx`) and the number of adverse effects (`num_effects`).

3. **Mann-Whitney U Test**:  
   Compare the age distributions of the Drug and Placebo groups, as normality assumptions were not met.

4. **Normality Tests**:  
   Shapiro-Wilk tests were conducted to assess the normality of age distributions in treatment groups.

---

## Key Findings

1. **Adverse Effects Proportion**:  
   A two-proportion Z-test was performed to evaluate whether the rate of adverse effects differs between Drug and Placebo groups. The p-value obtained determines the statistical significance.

2. **Number of Adverse Effects**:  
   A Chi-Square test of independence revealed whether the treatment group and the count of adverse effects are associated.

3. **Age Distribution**:  
   The age distributions of the Drug and Placebo groups were compared using a Mann-Whitney U test due to non-normality in data.

---

## Visualizations

- **Histogram of Age by Treatment Group**:  
  A visual comparison of age distributions in Drug and Placebo groups, colored by treatment type.

- **Adverse Effects Distribution**:  
  Graphical summaries of the presence and number of adverse effects.
