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
Raw Data: 

1. AD-CountyMostRecentYearsData 
Columns: County Name,Priority Area Number,Priority Area,Indicator Number,Indicator,Event Count/Rate, ,Percentage/Rate/Ratio,Lower Limit of 95% CI,Upper Limit of 95% CI,Data Comments,Data Years,Date Source
Column Meaning: Name of the county, Priority Area #, Priority Area name, Indication number, Asthma emergency department visit rate per 10,000 for different age groups, Count of emergency department visits, Lower Limit of 95% CI, Upper Limit of 95% CI, Data Comments, 2018-2020 data years, Source of the data

2. Annual_AQI_By_County_2018 
Columns: "State","County","Year","Days with AQI","Good Days","Moderate Days","Unhealthy for Sensitive Groups Days","Unhealthy Days","Very Unhealthy Days","Hazardous Days","Max AQI","90th Percentile AQI","Median AQI","Days CO","Days NO2","Days Ozone","Days PM2.5","Days PM10"
Column Meaning: Name of the state, Name of the county, Year, Days with recorded AQI, No. of Good days, No. of Moderate Days, No. of days which are unhealthy for sensitive groups, No. of days with are unhealthy for all, No. of days which are very unhealthy for all, No. of extremely unhealthy days, Maximum Qir Quality Index recorded in 2018, Median of Air Quality Index recorded in 2018, Days with Carbon Monoxide recorded in 2018, Days with Nitrogen Oxide recorded in 2018, Days with level of Ozone Recorded in 2018, Days with PM2.5 recorded in 2018, Days with PM10 recorded in 2018

3. Annual_AQI_By_County_2019
Columns: "State","County","Year","Days with AQI","Good Days","Moderate Days","Unhealthy for Sensitive Groups Days","Unhealthy Days","Very Unhealthy Days","Hazardous Days","Max AQI","90th Percentile AQI","Median AQI","Days CO","Days NO2","Days Ozone","Days PM2.5","Days PM10"
Column Meaning: Name of the state, Name of the county, Year, Days with recorded AQI, No. of Good days, No. of Moderate Days, No. of days which are unhealthy for sensitive groups, No. of days with are unhealthy for all, No. of days which are very unhealthy for all, No. of extremely unhealthy days, Maximum Qir Quality Index recorded in 2019, Median of Air Quality Index recorded in 2019, Days with Carbon Monoxide recorded in 2019, Days with Nitrogen Oxide recorded in 2019, Days with level of Ozone Recorded in 2019, Days with PM2.5 recorded in 2019, Days with PM10 recorded in 2019 

4. Annual_AQI_By_County_2020
Columns: "State","County","Year","Days with AQI","Good Days","Moderate Days","Unhealthy for Sensitive Groups Days","Unhealthy Days","Very Unhealthy Days","Hazardous Days","Max AQI","90th Percentile AQI","Median AQI","Days CO","Days NO2","Days Ozone","Days PM2.5","Days PM10"
Column Meaning: Name of the state, Name of the county, Year, Days with recorded AQI, No. of Good days, No. of Moderate Days, No. of days which are unhealthy for sensitive groups, No. of days with are unhealthy for all, No. of days which are very unhealthy for all, No. of extremely unhealthy days, Maximum Qir Quality Index recorded in 2020, Median of Air Quality Index recorded in 2020, Days with Carbon Monoxide recorded in 2020, Days with Nitrogen Oxide recorded in 2020, Days with level of Ozone Recorded in 2020, Days with PM2.5 recorded in 2020, Days with PM10 recorded in 2020

5. Daily_42101_2020
Columns: "State Code", "County Code", "Site Num", "Parameter Code", "POC", "Latitude", "Longitude", "Datum", "Parameter Name", "Sample Duration", "Pollutant Standard", "Date Local", "Units of Measure", "event Type", "Observation County", "Observation Percent", "Arithmetic Mean", "1st Max Value", "1st Max Hour", "AQI", "Method Code", "Method Name", "Local Site Name", "Address", "State Name", "County Name", "City Name", "CBSA Name", "Date of Last Change"
Column Meaning: "The FIPS code of the state in which the monitor resides", "The FIPS code of the county in which the monitor resides", "A unique number within the county identifying the site", "The AQS code corresponding to the parameter measured by the monitor", "This is the “Parameter Occurrence Code” used to distinguish different instruments that measure the same parameter at the same site", "The monitoring site’s angular distance north of the equator measured in decimal degrees", "The monitoring site’s angular distance east of the prime meridian measured in decimal degrees", "The Datum associated with the Latitude and Longitude measures", "The name or description assigned in AQS to the parameter measured by the monitor. Parameters may be pollutants or non-pollutants", "The calendar date of the sample in Local Standard Time at the monitor", "The time of day that sampling began on a 24-hour clock in Local Standard Time", "The calendar date of the sample in Greenwich Mean Time", ""The time of day that sampling began on a 24-hour clock in Greenwich Mean Time", "The measured value in the standard units of measure for the parameter", "The unit of measure for the parameter. QAD always returns data in the standard units for the parameter. Submitters are allowed to report data in any unit and EPA converts to a standard unit so that we may use the data in calculations", "The Method Detection Limit. The minimum sample concentration detectable for the monitor and method. Note: if samples are reported below this level, they may have been replaced by 1/2 the MDL", "The total measurement uncertainty associated with a reported measurement as indicated by the reporting agency", "Sample values may have qualifiers that indicate why they are missing or that they are out of the ordinary. Types of qualifiers are: null data, exceptional event, natural events, and quality assurance. The highest ranking qualifier, if any, is described in this field", "An indication of whether the method used to collect the data is a federal reference method (FRM), equivalent to a federal reference method, an approved regional method, or none of the above (non-federal reference method)", "An internal system code indicating the method (processes, equipment, and protocols) used in gathering and measuring the sample. The method name is in the next column"",, ""The name of the state where the monitoring site is located, 
Processed Data:
Spatial Data: 


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
