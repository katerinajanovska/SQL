The "Chicago" project focuses on preparing and SQL querying data within the Visual Studio Code environment and its Jupyter Notebook extension. The initial .csv files were processed and imported into an SQLite database using the Pandas library. For SQL querying, I chose to use the SQL-Magic and DB-API interfaces.

The project is based on datasets freely available on the City of Chicago's website. The following data is used in the project:
  
  - **ChicagoCensusData.csv**
      - socio-economic indicators of the population valid for the period 2008 - 2012

  - **ChicagoCrimeData.csv**
      - crime records between 2001 - 2024
      - for the purposes of the analysis, records of acts that occurred after the beginning of the 2011/2012 school year were deleted
  
  - **ChicagoPublicSchools.csv**
      - identification data and success indicators for public schools in the city of Chicago for the 2011/2012 school year


The original datasets are large and a significant portion of the columns are not relevant for purpose of this project. To maintain clarity, the data model below includes analyzed columns only.

| census | crime | schools|
|------------|------------|------------|
| COMMUNITY_AREA_NUMBER | COMMUNITY_AREA_NUMBER | COMMUNITY_AREA_NUMBER |
| COMMUNITY_AREA_NAME | ID  | SCHOOL_ID |
| PER_CAPITA_INCOME | CASE_NUMBER| NAME_OF_SCHOOLS |
| HARDSHIP_INDEX| DATE  | HEALTHY_SCHOOL_CERTIFIED  |
| PERCENT_HOUSEHOLDS_BELOW_POVERTY| PRIMARY_TYPE| COMMUNITY_AREA_NAME  |
