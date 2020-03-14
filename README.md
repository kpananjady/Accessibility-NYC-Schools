# Accessibility-NYC-Schools

So far, I see a story here on Queens' superior accessibility. There is also a suggestion that NYC has made some quick improvements on the accessibility front. 

Roughly one in four schools has a rating of 10 across the city, signifying highly accessible spaces. In Queens, over a third of schools have a rating of 10. Queens also has a higher median rating than other boroughs! What is driving this trend?

44 percent of schools in this dataset are classified as "fully accessible," which includes ratings 9 and 10. In 2018, Advocates for Children of NY found that it was one in five. (https://www.advocatesforchildren.org/access) What happened here? 

__

Data source 1: New York Department of Education
https://nycdoe.sharepoint.com/sites/BAP/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FBAP%2FShared%20Documents%2FBuilding%20Accessibility%20Profile%20List&p=true&originalPath=aHR0cHM6Ly9ueWNkb2Uuc2hhcmVwb2ludC5jb20vOmY6L3MvQkFQL0VwdzItQUtwNUs1THZXQzZYTFQ3Tk80Qlo2NW1CYmljTHlOUXYzdUltN09uTVE_cnRpbWU9MlBpc0hKX0gxMGc


NOTE on the data: The above data was last updated in February 2020. It contains 1200 or so entries — which is less than the total number of public schools in NYC. I wonder why that is; but this is an important caveat for any finding here.

__

Analysis 1: https://github.com/kpananjady/Accessibility-NYC-Schools/blob/master/Accessibility%20in%20NYC%20schools.ipynb

I open up the file, use regex to extract the rating, geolocate the schools with Google's API, disaggregate the data by borough and look at the descripive statistics associated with each corresponding histogram. 

NOTE on the analysis: At the moment, this analysis treats schools rated 0 (not accessible) and schools rated 0+ (at least one entrance and a small area ae accessible) both as 0. (See the data dictionary for the difference: https://www.schools.nyc.gov/school-life/school-environment/building-accessibility) In this dataset, 0 and 0+ doesn't actually matter as there aren't any 0 ratings within. 

__

Data source 2: New York City shapefiles from NYC Open Data https://data.cityofnewyork.us/City-Government/Neighborhood-Tabulation-Areas-NTA-/cpf4-rkhq 

NOTE on the data: Use CRS projection W84:4326 for the coordinate system when mapping!

__

Analysis 2: https://github.com/kpananjady/Accessibility-NYC-Schools/blob/master/ratings-city-analysis.qgz; see results in Screen Shot 2020-03-13 at 9.47.22 PM.png at https://github.com/kpananjady/Accessibility-NYC-Schools/blob/master/Screen%20Shot%202020-03-13%20at%209.47.22%20PM.png

I have added a QJIS map of schools and their ratings across the city using my geolocated data and shapefiles. It clearly illustrates how Queens is doing better. Mapping will also allow me to check my data against demographic indicators in the census to see if there are patterns that account for ratings. 

NOTE on the analysis: If you have an idea of what I should check accessibility against on a neighborhood level to test correlation, please let me know!
