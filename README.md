# Modeling Public Skepticism Toward Weight-Loss Drugs Like Ozempic

## Overview

This project explores the demographic and attitudinal predictors of public skepticism toward weight-loss medications such as Ozempic. Using survey data from the Pew Research Center (American Trends Panel, Wave 142), I fit ordinal and partial proportional odds logistic regression models to understand what factors make people more likely to view these medications with greater skepticism or pessimism towards their potential impact on reducing obesity in America.

Link to project on RPubs: https://rpubs.com/architn01/1313806


##  Research Question

> What factors predict whether someone is skeptical of weight-loss medications like Ozempic? What factor predict whether someone is pessimistic regarding the potential impact weight-loss medications like Ozempic might have on reducing obesity in America? 

## Methods

- **Data Source:** Pew Research Center, ATP Wave 142 (2023)
- **Sample Size:** ~2,155 U.S. adults
- **Outcome Variables:**  
  - Perceived long-term impact of weight-loss medications (optimism vs. pessimism)  
  - Agreement that Ozempic is a good treatment option for individuals with obesity or other weight-related health issues (support vs. skepticism)

- **Key Predictors:**  
  - Gender  
  - Political affiliation  
  - Income  
  - Exposure to Ozempic-related information 
  - Belief in genetic causes of obesity  

- **Statistical Techniques:**  
  - Ordinal logistic regression (`MASS::polr`)  
  - Brant test to assess proportional odds (`brant`)  
  - Partial proportional odds models (`VGAM::vglm`)  
  - Model fit: McFadden’s and Nagelkerke’s pseudo R², AIC, likelihood ratio tests  
  - Predicted probability plots for interpretation

## Repository Contents
  - Raw data from Pew Research Center survey (ATP W142.csv)
  - Codebook for raw survey data (ATP W142 Codebook.xlsx)
  - Information about the methodology of the American Trends Panel survey (ATP W142 Methodology.pdf)
  - Cleaned dataset (ozempic_survey_data_clean.csv)
  - RMarkdown File (AmericanOzempicSurveydraft.rmd)
  - R code used for the project

## Key Findings

- People who are **more exposed to information about the drugs**, **identify as Democrats**, and **believe obesity has genetic causes** are significantly **less skeptical** of Ozempic.
- **Lower-income**, **Republican**, and **male** participants showed **greater skepticism** toward the medications.
- The partial proportional odds model provided better fit and more accurate estimates than a standard ordinal logistic regression.


## Skills Demonstrated

- R data wrangling and cleaning
- Ordinal and partial proportional odds modeling
- Model diagnostics (Brant test, AIC, pseudo R²)
- Interpretation of coefficients and predicted probabilities
- Reproducible reporting in R Markdown


---

## Author

**Archit Nangavaram**

Senior Undergraduate in Psychology minoring in Addiction Studies and Expressive Arts Therapy 

Email: archit.nangavaram01@utrgv.edu 

LinkedIn: https://www.linkedin.com/in/archit-nangavaram-10b899293/
