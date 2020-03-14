# Accessibility-NYC-Schools

Data source: New York Department of Education
https://nycdoe.sharepoint.com/sites/BAP/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FBAP%2FShared%20Documents%2FBuilding%20Accessibility%20Profile%20List&p=true&originalPath=aHR0cHM6Ly9ueWNkb2Uuc2hhcmVwb2ludC5jb20vOmY6L3MvQkFQL0VwdzItQUtwNUs1THZXQzZYTFQ3Tk80Qlo2NW1CYmljTHlOUXYzdUltN09uTVE_cnRpbWU9MlBpc0hKX0gxMGc


NOTE on the data: The above data was last updated in February 2020. It contains 1200 or so entries — which is less than the total number of public schools in NYC. I wonder why that is.

__

Analysis 1: https://github.com/kpananjady/Accessibility-NYC-Schools/blob/master/Accessibility%20in%20NYC%20schools.ipynb


I open up the file, use regex to extract the rating, geolocate the schools with Google's API, disaggregate the data by borough and look at the descripive statistics associated with each corresponding histogram. 

NOTE on the analysis: At the moment, this analysis treats schools rated 0 (not accessible) and schools rated 0+ (at least one entrance and a small area ae accessible) both as 0. I'll refine that going forward. Source: See the data dictionary for the difference: https://www.schools.nyc.gov/school-life/school-environment/building-accessibility

__

Analysis 2: https://github.com/kpananjady/Accessibility-NYC-Schools/blob/master/ratings-city-analysis.qgz; see results in Screen Shot 2020-03-13 at 9.47.22 PM.png at https://github.com/kpananjady/Accessibility-NYC-Schools/blob/master/Screen%20Shot%202020-03-13%20at%209.47.22%20PM.png

I have added a QJIS map of schools and their ratings across the city. It clearly illustrates how Queens is doing better. Mapping will also allow me to check my data against demographic indicators in the census to see if there are patterns that account for ratings. 

NOTE on the analysis: If you have an idea of what I should check accessiility against on a neighborhood level to test correlation, please let me know!
