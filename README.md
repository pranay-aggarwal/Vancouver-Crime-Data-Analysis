# Vancouver Crime Report Analysis

## Overview

This repository contains a data analysis project focused on studying crime report trends across different neighborhoods in Vancouver, using data from the Vancouver Police Department. The goal of this analysis is to assist law enforcement in identifying areas with a higher probability of criminal activity and optimizing resource allocation.

## Dataset

The dataset used in this analysis includes crime data from all available years, ranging from 2003 to 2022. The key columns used for analysis are:
- `TYPE`: Different categories of crimes reported, such as Theft from Vehicle, Homicide, Mischief, and Offence Against a Person.
- `YEAR`: The year in which the crime was reported.
- `NEIGHBOURHOOD`: Different neighborhoods in Vancouver for which the data is recorded, including West End, Strathcona, Mount Pleasant, and Fairview.

## Hypothesis Testing

The analysis primarily focuses on two specific crime types: "Theft from a Vehicle" and "Offence Against a Person" in the neighborhoods of Mount Pleasant and Strathcona. The hypothesis tests conducted are as follows:

1. Is the crime type of "Theft from a Vehicle" greater in Mount Pleasant than Strathcona?
   - Null Hypothesis (H0): Theft From Vehicle in Mount Pleasant = Strathcona
   - Alternative Hypothesis (H1): Theft From Vehicle in Mount Pleasant > Strathcona

2. Is the crime type of "Offence against a Person" greater in Strathcona than Mount Pleasant?
   - Null Hypothesis (H0): Offence against a person in Mount Pleasant = Strathcona
   - Alternative Hypothesis (H1): Offence against a person in Mount Pleasant < Strathcona

## Methodology

Two methods were used for hypothesis testing: bootstrap and asymptotic analysis. While both methods should yield similar results for categorical data, in this case, bootstrap analysis was deemed more appropriate due to the following reasons:
- Large sample size, making it representative of the population.
- Satisfying all underlying assumptions for bootstrap analysis.

## Results

Based on the analysis, the following conclusions were drawn:

- Theft from Vehicle crimes are significantly higher in Mount Pleasant compared to Strathcona.
- Offence Against a Person crimes are significantly higher in Strathcona compared to Mount Pleasant.

These findings have implications for law enforcement strategies, suggesting a need to focus on addressing theft from vehicle crimes in Mount Pleasant and addressing offences against persons in Strathcona.

## Limitations

- The dataset may have some underlying errors that contributed to unusual results, such as p-values of 0.
- Computational limitations restricted the number of bootstrap samples to 100.
- Population standard deviation was assumed to be the true population standard deviation due to working with a sample.


- Continuation of crime trend analysis beyond 2023 to account for potential changes in crime rates.
- More thorough data validation and cleaning to address potential errors in the dataset.
- The impact of economic stability on crime rates in Vancouver, especially post-COVID-19.

