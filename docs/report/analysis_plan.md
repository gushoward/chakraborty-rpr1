# Reproduction of Chakraborty 2021 analysis of unequal distribution of COVID-19 for people with disabilities

## Contributors

- Gus Howard\*, augustush@middlebury.edu, @gushoward, github.com/gushoward, Middlebury College

### Abstract

Chakraborty (2021) examines the relationship between COVID-19 incidence rates and the percentage of people with disabilities across U.S. counties, considering socio-demographic factors like race, ethnicity, poverty status, age, and sex. Using bivariate correlations and generalized estimating equation (GEE) models, the study finds significant positive associations between COVID-19 rates and socially vulnerable populations. This reproduction study aims to verify Chakraborty’s findings for policy, research, and educational purposes by replicating all analyses, including county-level COVID-19 distributions, statistical correlations, and GEE models. The data and code are publicly available on GitHub, ensuring transparency and accessibility for further study.


This is a reproduction study of 'Chakraborty, J. 2021. Social inequities in the distribution of COVID-19: An intra-categorical analysis of people with disabilities in the U.S. Disability and Health Journal 14:1-5. https://doi.org/10.1016/j.dhjo.2020.101007.'

The goeal of the replication is to understand the links between race/ethnicity and disability and COVID-19 rates.

### Original and Replication Study metadata

- `Key words`: COVID-19, Disability, Race/ethnicity, Poverty, Reproducibility
- `Subject`: Social and Behavioral Sciences: Geography: Geographic Information Sciences
- `Date created`: 3/01/2025
- `Spatial Coverage`: Continental US
- `Spatial Resolution`: US Counties
- `Spatial Reference System`: Contiguous USA Albers Equal Area projection EPSG:5070
- `Temporal Coverage`: From 1/22/2020 to 8/1/2020
- `Temporal Resolution`:  Rates were collected as one temporal unit.

## Study design

This is a reproduction study to understand the links between race/ethnicity and disability and COVID-19 rates.

## Materials and procedure

### Computational environment

I will use the R version 4.4.2 with the following packages: "tidycensus", "tidyverse", "downloader", "sf", "classInt", "readr",
  "here", "s2", "pastecs", "tmap", "SpatialEpi", "svDialogs",
  "geepack", "knitr", "kableExtra", "foreign", "broom", "dotwhisker", "dotenv"

### Data and variables

Metadat for the two data sources can be found at https://github.com/gushoward/chakraborty-rpr1/blob/main/data/metadata/metadata_covid.xml and https://github.com/gushoward/chakraborty-rpr1/blob/main/data/metadata/metadata_acs.xml. 


### Data transformations

Initial Study does not include Alaska, Hawaii, or Puerto Rico. Data on people with disabilities in poverty is derived from a different census table (C18130) than data on people with disabilities and age, race, ethnicity, age, and biological sex (S1810). 

The COVID-19 data includes an estimate of the total population (POP_ESTIMA) and confirmed COVID-19 cases (Confirmed). The COVID-19 case data expresses cumulative count of reported COVID-19 from 1/22/2020 to 8/1/2020. Versions of the data can be found at the John Hopkins CCSE COVID-19 Data Repository (https://github.com/CSSEGISandData/COVID-19).

## Discussion

The aim of this reproduction is to further measure the relationship between COVID-19 incidence rates and various demographic variables. The analysis will map the dispersal of COVID distribution at the county level, as well as using a Kulldorf statistics for relative risk mapping of COVID rates. This work can do well to influence policy and high-level decision making when it comes to at risk populations. 


## Integrity Statement

The author of this preregistration completed this preregistration to the best of their knowledge and that no other preregistration exists pertaining to the same hypotheses and research.

This report is based upon the template for Reproducible and Replicable Research in Human-Environment and Geographical Sciences, DOI:[10.17605/OSF.IO/W29MQ](https://doi.org/10.17605/OSF.IO/W29MQ)
