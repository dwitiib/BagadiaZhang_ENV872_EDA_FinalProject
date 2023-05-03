# BagadiaZhang_ENV872_EDA_FinalProject

## Summary

This project aims to analyze the direct impact of the levels of air quality in New York State based on county data with the current rate of Asthma infections in residents. Relationships between childhood asthma rates and air quality as well as childhood asthma rates and non-White population density are analyzed to determine whether they are correlated. Spatial distribution of childhood asthma rates, non-White population density, air quality, and major air pollutants are displayed.

## Investigators

Dwiti Bagadia, Student, dwiti@ad.unc.edu
Yue Zhang, Student, zhangyue@ad.unc.edu

## KeywordsCancel changes

Air Quality, Asthma, Air Pollution, New York State, Demographic

## Research Questions 

**Question 1**: Is there a relationship between air quality and asthma rate in New York State between 2018 and 2020?

**Question 2**: Is there a relationship between non-White population density and asthma rate in New York State between 2018 and 2020?

## Database Information

Asthma data was downloaded from New York State's Department of Health. Air quality data was from EPA website. Moreover, demographic data is from Social Explorer, it is a 5-year estimated data from American Community Survey. Processed datasets were wrangled by the investigators and written into the ProcessedData folder in the repository.

## Folder structure, file formats, and naming conventions 

Folders in this repository include: Output, Code, Data/Raw, & Data/Processed. Data files are all downloaded/processed into csv format and code is in both .Rmd files as well as .R files. Files are named to include whether they are raw or processed and they include the site in which the code or data is in reference to.

## Metadata

<For each data file in the repository, describe the data contained in each column. Include the column name, a description of the information, the class of data, and any units associated with the data. Create a list or table for each data file.> 



## Scripts and code

Wrangling code: 
1. DataWrangling_AsthmaRates: code for wrangling childhood asthma rates data
2. DataWrangling_Demographic: code for wrangling non-White population density data
3. DataWrangling_AirQuality: code for wrangling air quality data

Exploration code:
1. DataExploration_AsthmaAirQuality: code for visualizing trend between childhood asthma rates and air quality
2. DataExploration_AsthmaDemographic: code for visualizing trend between childhood asthma rates and 
non-White population density

Linear regression code:
1. LinearRegression_AsthmaAirQuality: code for generating linear model for childhood asthma rates and air quality
2. LinearRegression_AsthmaDemographic: code for generating linear model for childhood asthma rates and non-White population density

Spatial analysis code:
1. SpatialAnalysis: code for creating maps for childhood asthma rates, non-White population density, air quality, major air pollutants


## Quality assurance/quality control

None