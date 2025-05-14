# Title of Study



### Authors

- First Name Last Name\*, email address, @githubname, ORCID link, affiliated institution(s)
- First Name Last Name, email address, @githubname, ORCID link, affiliated institution(s)

\* Corresponding author and creator

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



#### Primary data source1 name

**Standard Metadata**

- `Abstract`: Brief description of the data source
- `Spatial Coverage`: Specify the geographic extent of your study. This may be a place name and link to a feature in a gazetteer like GeoNames or OpenStreetMap, or a well known text (WKT) representation of a bounding box.
- `Spatial Resolution`: Specify the spatial resolution as a scale factor, description of the level of detail of each unit of observation (including administrative level of administrative areas), and/or or distance of a raster GRID size
- `Spatial Reference System`: Specify the geographic or projected coordinate system for the study
- `Temporal Coverage`: Specify the temporal extent of your study---i.e. the range of time represented by the data observations.
- `Temporal Resolution`: Specify the temporal resolution of your study---i.e. the duration of time for which each observation represents or the revisit period for repeated observations
- `Lineage`: Describe and/or cite data sources and/or methodological steps planned to create this data source.
  - sampling scheme, including spatial sampling
  - target sample size and method for determining sample size
  - stopping criteria for data collection and sampling (e.g. sample size, time elapsed)
  - de-identification / anonymization
  - experimental manipulation
- `Distribution`: Describe who will make the data available and how?
- `Constraints`: Legal constraints for *access* or *use* to protect *privacy* or *intellectual property rights*
- `Data Quality`: State any planned quality assessment
- `Variables`: For each variable, enter the following information. If you have two or more variables per data source, you may want to present this information in table form (shown below)
  - `Label`: variable name as used in the data or code
  - `Alias`: intuitive natural language name
  - `Definition`: Short description or definition of the variable. Include measurement units in description.
  - `Type`: data type, e.g. character string, integer, real
  - `Accuracy`: e.g. uncertainty of measurements
  - `Domain`: Expected range of Maximum and Minimum of numerical data, or codes or categories of nominal data, or reference to a standard codebook
  - `Missing Data Value(s)`: Values used to represent missing data and frequency of missing data observations
  - `Missing Data Frequency`: Frequency of missing data observations: not yet known for data to be collected

| Label | Alias | Definition | Type | Accuracy | Domain | Missing Data Value(s) | Missing Data Frequency |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| variable1 | ... | ... | ... | ... | ... | ... | ... |
| variable2 | ... | ... | ... | ... | ... | ... | ... |

#### Primary data source2 name

... same form as above...

#### Secondary data source1 name

**Standard Metadata**

- `Abstract`: Brief description of the data source
- `Spatial Coverage`: Specify the geographic extent of your study. This may be a place name and link to a feature in a gazetteer like GeoNames or OpenStreetMap, or a well known text (WKT) representation of a bounding box.
- `Spatial Resolution`: Specify the spatial resolution as a scale factor, description of the level of detail of each unit of observation (including administrative level of administrative areas), and/or or distance of a raster GRID size
- `Spatial Reference System`: Specify the geographic or projected coordinate system for the study
- `Temporal Coverage`: Specify the temporal extent of your study---i.e. the range of time represented by the data observations.
- `Temporal Resolution`: Specify the temporal resolution of your study---i.e. the duration of time for which each observation represents or the revisit period for repeated observations
- `Lineage`: Describe and/or cite data sources and/or methodological steps used to create this data source
- `Distribution`: Describe how the data is distributed, including any persistent identifier (e.g. DOI) or URL for data access
- `Constraints`: Legal constraints for *access* or *use* to protect *privacy* or *intellectual property rights*
- `Data Quality`: State result of quality assessment or state "Quality unknown"
- `Variables`: For each variable, enter the following information. If you have two or more variables per data source, you may want to present this information in table form (shown below)
  - `Label`: variable name as used in the data or code
  - `Alias`: intuitive natural language name
  - `Definition`: Short description or definition of the variable. Include measurement units in description.
  - `Type`: data type, e.g. character string, integer, real
  - `Accuracy`: e.g. uncertainty of measurements
  - `Domain`: Range (Maximum and Minimum) of numerical data, or codes or categories of nominal data, or reference to a standard codebook
  - `Missing Data Value(s)`: Values used to represent missing data and frequency of missing data observations
  - `Missing Data Frequency`: Frequency of missing data observations

| Label | Alias | Definition | Type | Accuracy | Domain | Missing Data Value(s) | Missing Data Frequency |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| variable1 | ... | ... | ... | ... | ... | ... | ... |
| variable2 | ... | ... | ... | ... | ... | ... | ... |

#### Secondary data source2 name

... same form as above...

### Prior observations  

Prior experience with the study area, prior data collection, or prior observation of the data can compromise the validity of a study, e.g. through p-hacking.
Therefore, disclose any prior experience or observations at the time of study pre-registration here, with example text below:

At the time of this study pre-registration, the authors had _____ prior knowledge of the geography of the study region with regards to the ____ phenomena to be studied.
This study is related to ____ prior studies by the authors

For each primary data source, declare the extent to which authors had already engaged with the data:

- [ ] no data collection has started
- [ ] pilot test data has been collected
- [ ] data collection is in progress and data has not been observed
- [ ] data collection is in progress and __% of data has been observed
- [ ] data collection is complete and data has been observed. Explain how authors have already manipulated / explored the data.

For each secondary source, declare the extent to which authors had already engaged with the data:

- [ ] data is not available yet
- [ ] data is available, but only metadata has been observed
- [ ] metadata and descriptive statistics have been observed
- [ ] metadata and a pilot test subset or sample of the full dataset have been observed
- [ ] the full dataset has been observed. Explain how authors have already manipulated / explored the data.

If pilot test data has been collected or acquired, describe how the researchers observed and analyzed the pilot test, and the extent to which the pilot test influenced the research design.

### Bias and threats to validity

Given the research design and primary data to be collected and/or secondary data to be used, discuss common threats to validity and the approach to mitigating those threats, with an emphasis on geographic threats to validity.

These include:
  - uneven primary data collection due to geographic inaccessibility or other constraints
  - multiple hypothesis testing
  - edge or boundary effects
  - the modifiable areal unit problem
  - nonstationarity
  - spatial dependence or autocorrelation
  - temporal dependence or autocorrelation
  - spatial scale dependency
  - spatial anisotropies
  - confusion of spatial and a-spatial causation
  - ecological fallacy
  - uncertainty e.g. from spatial disaggregation, anonymization, differential privacy

### Data transformations

Describe all data transformations planned to prepare data sources for analysis.
This section should explain with the fullest detail possible how to transform data from the **raw** state at the time of acquisition or observation, to the pre-processed **derived** state ready for the main analysis.
Including steps to check and mitigate sources of **bias** and **threats to validity**.
The method may anticipate **contingencies**, e.g. tests for normality and alternative decisions to make based on the results of the test.
More specifically, all the **geographic** and **variable** transformations required to prepare input data as described in the data and variables section above to match the study's spatio-temporal characteristics as described in the study metadata and study design sections.
Visual workflow diagrams may help communicate the methodology in this section.

Examples of **geographic** transformations include coordinate system transformations, aggregation, disaggregation, spatial interpolation, distance calculations, zonal statistics, etc.

Examples of **variable** transformations include standardization, normalization, constructed variables, imputation, classification, etc.

Be sure to include any steps planned to **exclude** observations with *missing* or *outlier* data, to **group** observations by *attribute* or *geographic* criteria, or to **impute** missing data or apply spatial or temporal **interpolation**.

### Analysis

Describe the methods of analysis that will directly test the hypotheses or provide results to answer the research questions.
This section should explicitly define any spatial / statistical *models* and their *parameters*, including *grouping* criteria, *weighting* criteria, and *significance thresholds*.
Also explain any follow-up analyses or validations.

## Results

Describe how results are to be presented.

## Discussion

Describe how the results are to be interpreted *vis a vis* each hypothesis or research question.

## Integrity Statement

Include an integrity statement - The authors of this preregistration state that they completed this preregistration to the best of their knowledge and that no other preregistration exists pertaining to the same hypotheses and research.
If a prior registration *does* exist, explain the rationale for revising the registration here.

## Acknowledgements

- `Funding Name`: name of funding for the project
- `Funding Title`: title of project grant
- `Award info URI`: web address for award information
- `Award number`: award number

This report is based upon the template for Reproducible and Replicable Research in Human-Environment and Geographical Sciences, DOI:[10.17605/OSF.IO/W29MQ](https://doi.org/10.17605/OSF.IO/W29MQ)

## References
