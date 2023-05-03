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


5. Daily_42101_2020, Daily_42401_2020, Daily_42602_2020, Daily_44201_2020, Daily_81102_2020, Daily_88502_2020
Columns: "State Code", "County Code", "Site Num", "Parameter Code", "POC", "Latitude", "Longitude", "Datum", "Parameter Name", "Sample Duration", "Pollutant Standard", "Date Local", "Units of Measure", "event Type", "Observation County", "Observation Percent", "Arithmetic Mean", "1st Max Value", "1st Max Hour", "AQI", "Method Code", "Method Name", "Local Site Name", "Address", "State Name", "County Name", "City Name", "CBSA Name", "Date of Last Change"

Column Meaning: "The FIPS code of the state ", "The FIPS code of the county", "A unique number within the county identifying the site", "The AQS code corresponding to the parameter measured by the monitor", "This is the “Parameter Occurrence Code", "The monitoring site’s angular distance north of the equator measured in decimal degrees", "The monitoring site’s angular distance east of the prime meridian measured in decimal degrees", "The Datum associated with the Latitude and Longitude measures", "The name or description assigned in AQS to the parameter measured by the monitor", "The averaging period", "A description of the ambient air quality standard rules used to aggregate statistics", "The calendar date of the average in Local Standard Time at the monitor", "The unit of measure for the parameter", "Indicates whether data measured during exceptional events are included in the summary", "Number of observations taken during a day", "The average (arithmetic mean) value for the day", "The highest value for the day", "The hour when the highest value for the day was taken", ""The Air Quality Index for the day for the pollutant", "An internal system code indicating the method", "A short description of the processes, equipment, and protocols used in gathering and measuring the sample", "The name of the site", "Approximate street name of the monitoring site", "Name of the State"< "Name of the County", "Name of the City", "Name of the core bases statistical area", ""The date the last time any numeric values in this record were updated in the AQS data system". 


6. R13366951_SL050
Columns: Geo_FILEID,Geo_STUSAB,Geo_SUMLEV,Geo_GEOCOMP,Geo_LOGRECNO,Geo_US,Geo_REGION,Geo_DIVISION,Geo_STATECE,Geo_STATE,Geo_COUNTY,Geo_COUSUB,Geo_PLACE,Geo_TRACT,Geo_BLKGRP,Geo_CONCIT,Geo_AIANHH,Geo_AIANHHFP,Geo_AIHHTLI,Geo_AITSCE,Geo_AITS,Geo_ANRC,Geo_CBSA,Geo_CSA,Geo_METDIV,Geo_MACC,Geo_MEMI,Geo_NECTA,Geo_CNECTA,Geo_NECTADIV,Geo_UA,Geo_CDCURR,Geo_SLDU,Geo_SLDL,Geo_ZCTA5,Geo_SUBMCD,Geo_SDELM,Geo_SDSEC,Geo_SDUNI,Geo_UR,Geo_PCI,Geo_PUMA5,Geo_GEOID,Geo_NAME,Geo_BTTR,Geo_BTBG,Geo_QName,Geo_FIPS,Geo_AREALAND,Geo_AREAWATR,Geo_PLACESE,Geo_UACP,Geo_VTD,Geo_ZCTA3,Geo_TAZ,Geo_UGA,Geo_PUMA1,SE_A00001_001,SE_A00003_001,SE_A00003_002,SE_A00003_003,SE_A03001_001,SE_A03001_002,SE_A03001_003,SE_A03001_004,SE_A03001_005,SE_A03001_006,SE_A03001_007,SE_A03001_008

Column Meaning: "File identification","State Postal Abbreviation","Summary Level","Geographic Component","Logical Record Number","US","Census Region","Census Division","State (Census Code)","State (FIPS Code)","County of current residence","County Subdivision (FIPS)","Place (FIPS Code)","Census Tract","Block Group","Consolidated City","American Indian Area/Alaska Native Area/ Hawaiian Home Land (Census)","American Indian Area/Alaska Native Area/ Hawaiian Home Land (FIPS)","American Indian Trust Land/Hawaiian Home Land Indicator","American Indian Tribal Subdivision (Census)","American Indian Tribal Subdivision (FIPS)","Alaska Native Regional Corporation (FIPS)","Metropolitan and Micropolitan Statistical Area","Combined Statistical Area","Metropolitan Statistical Area- Metropolitan Division","Metropolitan Area Central City","Metropolitan/Micropolitan Indicator Flag","New England City and Town Area","New England City and Town Combined Statistical Area","New England City and Town Area Division","Urban Area","Current Congressional District ***","State Legislative District Upper","State Legislative District Lower","5-digit ZIP Code Tabulation Area","Subminor Civil Division (FIPS)","State-School District (Elementary)","State-School District (Secondary)","State-School District (Unified)","Urban/Rural","Principal City Indicator","Public Use Microdata Area – 5% File","Geographic Identifier","Area Name","Tribal Tract","Tribal Block Group","Qualifying Name","FIPS","Area (Land)","Area (Water)","Place (State FIPS + Place FIPS)","Urban Area Central Place","Voting District","ZIP Code Tabulation Area (3-digit)","Traffic Analysis Zone","Urban Growth Area","Public Use Microdata Area - 1% File","Total Population","Area Total:","Area Total: Area (Land)","Area Total: Area (Water)","Total Population:","Total Population: White Alone","Total Population: Black or African American Alone","Total Population: American Indian and Alaska Native Alone","Total Population: Asian Alone","Total Population: Native Hawaiian and Other Pacific Islander Alone","Total Population: Some Other Race Alone","Total Population: Two or More Races"


Processed Data:

1. NY_AQ_Processed1
Columns: "County","BadDaysRate"
Column Meaning: "Name of the County", "Rate of number of bad days recorded in the county in the years 2018-2020"

2. NY_Asthma_Processed1
Columns: "County","Visit Rate"
Column Meaning: "Name of the County", "Rate of asthma patients that visited the ER in the county"

3. NY_CO_Processed
Columns: "County", "Mean CO"
Column Meaning: "Name of the County", "Average of Carbon Monoxide recorded"

4. NY_Demographic_Processed
Columns: "County", "NonWhiteDens"
Column Meaning: "Name of the County", "Rate of Non white population in the county"

5. NY_NO2_Processed
Columns: "County", "MeanNO2"
Column Meaning: "Name of the County", "Average of Nitrogen Dioxide recorded"

6. NY_Ozone_Processed
Columns: "County", "MeanOzone"
Column Meaning: "Name of the County", "Average of Ozone recorded"

7. NY_PM10_Processed
Columns: "County", "MeanPM10"
Column Meaning: "Name of the County", "Average of PM10 recorded"

8. NY_PM25_Processed
Columns: "County", "MeanPM25"
Column Meaning: "Name of the County", "Average of PM2.5 recorded"

9. NY_SO2_processed
Columns: "County", "MeanSO2"
Column Meaning: "Name of the County", "Average of Sulphur Dioxide recorded"


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
