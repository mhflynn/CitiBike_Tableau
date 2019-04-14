# CitiBike_Tableau 

#### This project implements a Tableau dashboard for the CitiBike program in New York City, based on data for the year 2018. There are 12 data sets, csv files, 1 for each month of 2018, that contain information for every bike trip. There is a dashboard for to view ridership characteristics, station utilization and program usage information. 

#### A MS Powerpoint presentation is also available in the repository for quick view of material without opening the Tableau workbook

## Setup
 To view the Tableau workbook, first copy or clone the CitiBike_Tableau repository. Prior to opening the workbook, the data files in folder data/zip need to be uncompressed/unzipped into the data folder. For Mac users, make "data" folder the working directory, then run the "unzip_raw_data.sh" shell file with command "source unzip_raw_data.sh". For PC users, please manually unzip each zip file in the "data/zip" folder and place in the "data" folder. 

## Dashboards
Open the BikeDataDashboard.twb Tableau workbook. The dashboards are best viewed in presentation mode. 

### Ridership Dashboard
This dashboard provides an overview of the ridership characteristics for 2018. Data is summarized in tabular and graph form, highlighting overall number of trips, highlighted by User Type [Customer / Subscriber] and Gender [Male / Female / Unknown] and Age of rider. 

Notable characteristics :
* The majority of the ridership are Subscribers to the program, making up 89% of the ridership. Customers are are assumed to be non-subscribers and hence explains poor data characteristics for that group. The majority of the Customers are identified as "Unknown" gender, and also make up the majority of "Unknown" gender across all riders. Recommend attention to information gathering mechanisms for non-subscribers.
* Likewise for Birth Year, the majority of Customers have birth year of 1969, which assumed to indicate the information was not provided. There is also significant number of Subscribers with Birth Year of 1969, recommend effort to formally identify this value as indicative of no data or to collect the correct information from the Subscribers.
* The majority of riders are between the ages 25 to 40.
* As expected, the number of rides is significantly higher in the warmer months of the year.

### Usage Dashboard
This dashboard provides and overview of the system usage by time of day and time duration of each trip. Data is broken out by User Type [Customer / Subscriber] and Gender [Male / Female / Unknown]. 

Notable characteristics :
* The majority of trips are in daylight hours. 
* The trip duration is fairly consistent, independent of time of day, with exception of an anomaly for the hours between 3:00 and 4:00am. This is speculated to be maintenance related, where bike may be taken offline for upkeep and repair

### Station Dashboard
This dashboard provides view of the most utilized and least utilized stations for starting and ending a trip. 

Notable observations :
* Very bottom ranked stations appear to be maintenance related, although this information is to excluded from the datasets. The fact that that there are very few, indicates for the most part, the maintenance related trips are being exclude from the data, but some still appear. 
* For low rank stations that are not maintenance related, recommend to reevaluate their utility. 

### Station Maps
Two maps are provided as geographical overview of the station usage. Stations are indicate by circles whose size and color indicate number of trips. The first map is view of station/trips for 2018, the second map is view of station/trips by month. The view the monthly information, use the "Month" dialog box to select a month or use > button to animated view from January to December 2018. 

#### Worksheets
Following the dashboards and usage maps, are the individual Tableau work sheets supporting the dashboards. There are additional worksheets not included in the dashboards for view in greater detail. 
