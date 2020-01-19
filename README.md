# SMU_ETL_Team_4
# ETL Project

### Project Summary
We are performing ETL on datasets for opioid overdose deaths in all US states. We downloaded data relevant to opioid overdose deaths, all-drug overdose deaths, annual percent rate changes, and prescriber information per state in 2014. 

overdoses.csv | prescriber-info.csv | raw_data.csv

https://www.kaggle.com/apryor6/us-opiate-prescriptions#prescriber-info.csv

https://www.cdc.gov/media/releases/2015/p1218-drug-overdose.html

### Data ETL
We extracted our csv files into pandas dataframes and selected columns to keep and rename for analysis. We checked for duplicate and null values in all csvs; only two rows from the age_adjusted_rate dataframe dropped. We created tables in pgAdmin with SQL queries and established a connection to PostgreSQL to load our final dataframes. We confirmed the upload by taking SQL queries in Jupyter Notebook. 

### Analysis of State Overdose Deaths and Prescriber Records in 2014 
We downloaded and viewed overdoses.csv and prescriber-info.csv, and extracted each csv into a Pandas dataframe. Within our overdoses data, we analyzed deaths per state and population per state to calculate the deaths per capita. We added a Matplotlib bar graph to display total populations by state. Within our prescriber data, we grouped prescriber's gender and specialty by state. We merged both dataframes to view opioid deaths, total population, prescriber gender, and prescriber specialty by state. We needed to rename column headers, remove irrelevant columns, aggregate by state, and analyze the results using descriptive functions. 

### Data Limitations
Our overdose and prescriber data is aggregated by state, rather than location. We are unable to identify if overdoses and prescription rates are correlated by city, county, or region. 
Our data only identifies registered medical providers and not illicit street-corner dealers. An unknown number of opioid overdoses could be attributed to 'dirty' opioids tainted with other illicit drugs. 
Our data does not identify the cause of injury that generated a need for opioid medication or whether the patient's career carries a higher statistical risk of injury, i.e. construction. 
Our data does not identify the month of death to view if rates of death increase during certain times of year. 

TEAM MEMBERS:
[Ahmed Gurbuz](https://github.com/ahmedgurbuz "Ahmed Gurbuz") </br>
[Hena Venu](https://github.com/ "Hena Venu") </br>
[Issac Vilchis](https://github.com/Issac-Vilchis "Issac Vilchis") </br>
[Marina Staber](https://github.com/stabm "Marina Staber") </br>
[Mike Hughes](https://github.com/brokerace "Mike Hughes") 
