# The state of accessibility to public psychological health in Italy
This folder contains the project for the course "Geospatial Analysis and Representation for Data Science" on the state of accessibility to public mental health care in Italy.

## Aim of the project
The project was created with the idea of investigating the accessibility of public mental health care and treatment services in Italy. 
The aim is to map physical places of access to free (or subsidized) psychological and psychiatric therapies, establish their geographical distribution across provinces and in cities, compare territorial units that are more or less served, and investigate effects/interactions with other geo-referenced socio-demographic variables.
## Structure
Specifically, I will first use the Consultori Centers, and then hospital and clinical health facilities marked as such on OpenStreetMap, as proxies of public facilities where psychological care and treatment can be received. After geolocating these facilities, and plotting them on maps of the national territory divided by provinces (main_geospatial, data loading-processing-visualization section), I will develop:
- A city-scale analysis of the places of care near a point of the user's choice with the routes to get there (main_geospatial, Street network analysis section).
- a comparative analysis between provinces and finally a statistical analysis with the aim of relating service availability and psychological distress to other variables, attempting to investigate their spatial correlation dimension as well (Rmd).
## How to run the code
-- For the Python part, it is possible to run the code directly following the notebook (main_geospatial), all data can be accessed from the given "data" folder or at the given links (for some particularly time-consuming cells, intermediate results are saved to prevent the user from having to run those cells). The requirements are all reported. installed and loaded in the first few cells.
The project was done in Colab; its use is recommended to ensure full functionality.

-- For the R part, it can be useful to download the html file for an immediate rendering, including parts of text and maps, of the spatial analysis using autocorrelation measures and regression models. To run the code, it is possible to directly follow the RMarkdown, all requirements are listed, installed, and loaded in the first chunk.
## Data sources
The following datasets are stored in the “data” folder
-	Consultori dataset, provided by the Ministry of Health, under Italian Open Data Licence.
-	Geographic data, provided by Istat, under Creative Commons - Attribution - 3.0 licence.
-	Population dataset (and regression_data dataset with other socio-demographic variables and indicators), provided by the "Health for All" database system by Istat (details in the R file). All datasets are stored and accessible in the “data” folder of the repository. To access the database system directly, a full guide is provided at https://www.istat.it/it/archivio/14562.
-	intermediate results about Consultori.

