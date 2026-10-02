# Seattle Neighborhood Livability Analysis

An exploratory data analysis of neighborhood livability in Seattle, examining crime, education and demographics, economic conditions, and access to public amenities from 2016–2024.

## Overview

This project investigates how different factors contribute to quality of life across Seattle neighborhoods. We combine multiple publicly available datasets to examine patterns in safety, education, demographics, economic hardship, and access to public facilities.

The analysis was developed for INFO 201 at the University of Washington by:

* Brooks Kahsai
* Njeri Kimani
* Lunjia Dai
* Anika Indurkar
* Andrew Tomoiaga

## Research Questions

The project focuses on four questions:

1. Crime: How did crime rates change between 2016 and 2024, and how did the proportions of different crime types vary across Seattle neighborhoods?
2. Education & Demographics: How do education and demographic distributions intersect with income, crime rates, and access to public amenities?
3. Economic Conditions: Is there a relationship between unemployment and deep poverty among working-age adults ages 20–64?
4. Public Amenities: How does neighborhood location influence access to public facilities?

These questions were designed to provide a multidimensional view of neighborhood livability rather than evaluating neighborhoods using a single metric.

## Data Sources

The analysis combines four primary categories of publicly available data:

Category	Source	Purpose
Crime	Seattle Police Department / Data.gov	Analyze crime trends and neighborhood safety
Education & Demographics	U.S. Census Bureau, ACS 5-year estimates / Data.gov	Examine education, race, and demographic patterns
Economic Indicators	U.S. Census Bureau, ACS 5-year estimates / Data.gov	Analyze unemployment, income, and deep poverty
Public Amenities	City of Seattle GIS / Data.gov	Measure access to urban centers and parks

## Methodology

The project uses R for data cleaning, transformation, analysis, and visualization.

### Key steps include:

* Importing multiple Seattle neighborhood datasets
* Cleaning and filtering records relevant to the analysis
* Converting date fields and extracting years for temporal analysis
* Grouping Seattle’s detailed neighborhood designations into broader NeighborhoodGroup categories
* Calculating crime rates relative to population
* Categorizing crime into broader groups such as violent, property, and other crimes
* Calculating unemployment and deep-poverty rates for adults ages 20–64
* Combining park and urban-center counts to measure public amenities
* Normalizing amenity counts by population
* Creating visualizations to compare patterns across neighborhoods

The crime dataset contains more than 1.4 million reported incidents, while the amenities analysis calculates the number of amenities per 10,000 residents.

## Key Findings

### Crime

Crime patterns varied substantially across Seattle neighborhoods and by crime type. Assaults represented a major component of violent crime, particularly in areas such as SODO/Duwamish and Downtown/Core. More residential neighborhoods, including Queen Anne/Magnolia, Eastlake, and Capitol Hill, showed lower levels of violent crime, while property crime remained comparatively prevalent.

### Education & Demographics

Education enrollment patterns differed by education level, with preschool and kindergarten enrollment generally lower than enrollment from primary education through post-secondary education. The analysis also found demographic differences between neighborhoods while observing relatively similar education enrollment patterns across racial groups.

### Unemployment & Poverty

The analysis found a positive relationship between unemployment among adults ages 20–64 and deep poverty rates across Seattle neighborhoods. This is an association at the neighborhood level and does not establish that unemployment causes deep poverty.

### Public Amenities

Public amenities varied considerably when measured relative to neighborhood population. South Seattle and Downtown/Core had some of the highest amenities rates, while areas such as Queen Anne/Magnolia and the Central District had lower rates under the project’s definition of amenities.

### Limitations

Several limitations affect how the results should be interpreted:

* Neighborhoods had to be manually grouped into broader categories, which can obscure differences within individual areas.
* Population data was not always available on a year-by-year basis, requiring approximations when calculating some crime rates.
* Some crime records were classified broadly as "All Other", limiting more detailed crime analysis.
* Education and demographic datasets did not always align cleanly with neighborhood population groupings.
* The amenities analysis excluded Seattle Parks and Recreation (SPR) properties from the parks dataset used.
* Counting amenities does not account for differences in their size, quality, accessibility, or actual usage.
* Neighborhood-level correlations cannot establish causation.

## Tools & Technologies

* R
* tidyverse
* ggplot2
* Data cleaning and transformation
* Statistical and descriptive analysis
* Data visualization

## Future Work

Future analysis could improve the study by:

* Using year-specific population estimates to calculate more precise crime rates
* Expanding crime categories beyond broad violent/property classifications
* Incorporating additional economic, education, housing, and demographic variables
* Using more consistent neighborhood definitions across datasets
* Incorporating a more comprehensive inventory of public amenities, including Seattle Parks and Recreation facilities
* Examining trends across multiple years to distinguish persistent patterns from temporary changes
* Incorporating measures of actual accessibility, quality, and usage of public facilities

Project Report

The accompanying HTML report contains the full analysis, visualizations, discussion, and R code used in the project.
