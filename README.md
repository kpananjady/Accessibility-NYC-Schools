# Accessibility-NYC-Schools

Data source: New York Department of Education
https://nycdoe.sharepoint.com/sites/BAP/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FBAP%2FShared%20Documents%2FBuilding%20Accessibility%20Profile%20List&p=true&originalPath=aHR0cHM6Ly9ueWNkb2Uuc2hhcmVwb2ludC5jb20vOmY6L3MvQkFQL0VwdzItQUtwNUs1THZXQzZYTFQ3Tk80Qlo2NW1CYmljTHlOUXYzdUltN09uTVE_cnRpbWU9MlBpc0hKX0gxMGc


NOTE on the data: The above data was last updated in February 2020. It contains 1200 or so entries — which is less than the total number of public schools in NYC. I wonder why that is.

I open up the file, use regex to extract the rating, geolocate the schools with Google's API, disaggregate the data by borough and look at the descripive statistics associated with each corresponding histogram. 

NOTE on the analysis: At the moment, this analysis treats schools rated 0 (not accessible) and schools rated 0+ (at least one entrance and a small area ae accessible) both as 0. I'll refine that going forward. Source: See the data dictionary for the difference: https://www.schools.nyc.gov/school-life/school-environment/building-accessibility

I will add a QJIS map of schools and their rating across the city soon to see if there is a pattern there. This will also allow me to check my data against demographic indicators in the census to see if there are patterns there as well.
