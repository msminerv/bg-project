# Cleaning


[Burning Glass technologies](https://www.burning-glass.com/), the provider from whom we purchase these data, specialises in collecting and organising labor market data (job ads and the like), from a variety of sources, and especially through web crawlers.

# Table of Contents

1. Getting the Data
2. Extracting
3. Cleaning
4. Getting Specific Companies
5. Getting NAICS Code
6. Salary Data
7. Merge Glassdoor and BG data


## 1. Getting the Data

The way in which we received the data was by obtaining access to a remote source of files that continuously gets updated. These files can be accessed, to my knowledge, via two ways and both will need a username and password. Please contact Victoria Sevcenko for the details, should you become involved in this project at a later stage.

### First way to access the data

1. Download [Filezilla](https://filezilla-project.org/)
2. Use the username and password for the account to log in to the server `transfer.burning-glass.com`
3. Navigate to the folder `HistoricalFeed/Jobs/US/Add`
4. Select the data you want and move it to your folder of choice.

### Second way to access the data

1. Open up your terminal (MacOS or Linux only)
2. Type `ftp -p transfer.burning-glass.com`
3. Enter the `username`
4. Enter the `password`
5. Navigate to the folder `cd HistoricalFeed/Jobs/US/Add`
6. Go into the year you would like to get data for e.g. `cd 2020`
7. Type `binary`
8. Type `prompt`
9. Type `mget *` and all of the files for that folder will begin to download  
NB: You can type the name of a single file or multiple as well.

## Third way to access the data
1. Enter the shared Jupyter Notebook
2. Access ".ipynb"
3. Description of steps are in the code
