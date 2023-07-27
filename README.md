# EDA-Project-One-Group-6
First Project of EDA 

Project Title: Immigrant's status in Canada

Jihye Yoon_

My part was visulizing which regions in Ontario has the highest number of immigrants, non-immigrants, and non-permanent residents.
Torotto has the highest number of immigrants, non immigrants and non permanent residents.

I used dataset from StatCanada and the dataset shows the population of immigrants, non immigrants and non permanent residents in cities in Ontario. 

This is how I cleand, manuplated and visualized the data.

Step#1. read_csv
The CSV file I have downloaded represents the immigration data for all provinces in Canada. To focus specifically on the Ontario region, I clean the data and extract records corresponding to Ontario from the GEO column.

Step#2. Create a dataframe
I retrieve specific columns from the Ontario region's data. The required columns include 'Region Name, 'Non-Immigrant Count, 'Immigrant Count, 'Immigrant Count Before 2001, 'Immigrant Count Between 2001 and 2005, 'Immigrant Count Between 2006 and 2011, 'Immigrant Count Between 2011 and 2015, 'Immigrant Count Between 2016 and 2021, and 'Non-Permanent Resident Count.  I also need
'Latitude, Longitude' to make a map with cleand data. 

Step#3.
To obtain the latitude and longitude for the desired locations, I utilize my API from Geoapify.com. However, the original region names were listed as 'region name, Ont.' in the dataset. To address this, I use the replace function to change 'Ont.' to 'Ontario' in the region names before retrieving the necessary information.

Step#4.
To enhance data visualization on the map, I perform data type conversions. All values in the dataset were converted to 'int64', and the latitude and longitude columns were changed to 'float64' for more accurate positioning on the map.I utilized hvplot to visualize the data on the map.

Step#5
After exploring the data, I identified that Toronto has the highest immigrant count, non-immigrant count, and non-permanent resident count. To present this information in a visually informative way, I created a pie chart that shows the proportion of each category. Similarly, I performed the same analysis for Ottawa, the region with the second-highest immigrant count, non-immigrant count, and non-permanent resident count, and represented the results using a pie chart as well.



