# EDA-Project-One-Group-6

First Project of EDA 

**Population Growth in Ontario Regions: Explore the population growth rates and trends in different regions of Ontario. Identify areas with the highest and lowest population growth and investigate potential factors contributing to these variations.**

**Team Members**

Sanjeev Chiplunkar,  Priyanshi Gajjar,  Jihye Yoon,  Sughra Shadab

**Summary**

The objective of this project is to analyze demographic data related to age, gender, region and year of immigrant status in Canada. The dataset used for this analysis is derived from the 2021 Counts statistics, which provide information on the population distribution across various age groups, genders, and immigrant categories. 

The project focuses on understanding the composition of the Canadian population based on age, gender, and immigration characteristics. It aims to provide insights into the distribution of the population in different age groups, gender categories, and immigrant statuses, including non-immigrants, immigrants, and non-permanent residents. 

The analysis will involve examining the data at provincial levels. The geographic breakdown includes Ontario as a whole and its individual areas. The provinces which we have considered in this study is Ontario.

**Division of Work** 

# Jihye

1. Which regions have the highest number of immigrants, non-immigrants, and non-permanent residents? 

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




# Sanjeev
 
2. Among which age groups are immigrants, non-immigrants, and non-permanent residents most prevalent? 
My part of the project was to collect data for different age groups among immigrants, non-immigrants, and non-permanent residents

Data Collection: After reviewing the data in the csv file. I started cleaning it up by removing first the NaN values and removing irrelevant columns. Cleaned up the columns names to make it more readable After that i grouped all the ages available in the data, and grouped them by regions as well focusing on Ontario

Data Analysis: Calculated the different age groups by immigrants, non-immigrants, and non-permanent residents. Also, filtered the data further to calculate the same data within toronto

Data Visualization: To visualize the data I used bar charts for immigrants, non-immigrants, and non-permanent residents in ontario and toronto .

The most significant age group was 15 years and older, more specifically the 25 to 65 group. Most of the numbers coming out of the Toronto region I did an analysis on the Ottawa region as well and found out that the age groups remain the same as in Toronto.

# Priyanshi 

3. Which gender constitutes a larger and lowest proportion of immigrants, non-immigrants, and non-permanent residents in Ontrio, Canada?

- My research focused on analyzing the gender distribution among immigrants, non-immigrants, and non-permanent residents in different regions of Ontario. To accomplish this, I accessed demographic data from reliable sources, such as government statistics and census data.

Here is a step-by-step guide detailing the process of the analysis:

1. Data Collection:
I examined official data sources that provided information on the population, immigration, and non-permanent residents in Ontario regions, primarily relying on the Canadian government's website and Statistics Canada. I obtained data on the gender distribution within each of these population categories in various regions of Ontario.

2. Data Preparation:
I carefully cleaned the data to remove any inconsistencies that could potentially affect the analysis. Subsequently, I organized the data in a structured format, making it easier to read and generate visualizations.

3. Data Analysis:
I first calculated the proportion of males and females in each category (immigrants, non-immigrants, non-permanent residents). Additionally, I compared the gender distribution across different categories to identify any significant variations.

4. Data Visualization:
To provide a clear and visual representation, I chose to use a Pie-chart for visualizing the gender distribution among immigrants, a Line graph for non-immigrants, and a Bar chart for non-permanent residents.

5. Interpretation and Analysis of Results:
After cleaning and analyzing the data from various perspectives and data frames, I successfully identified the top and bottom three provinces for male immigrants, non-immigrants, and non-permanent residents, as well as for female immigrants, non-immigrants, and non-permanent residents.

6. Toronto emerged as the predominant province for both men and women in all three categories, followed by Ottawa and Hamilton.
Conversely, Hawkesbury was the least explored province for both men and women in all three categories, with Kenora and Pembroke being the subsequent least represented provinces.

7. Investigation of Factors:
The next step in the research is to explore potential factors contributing to the observed variations. Factors such as economic opportunities, family reunification, education, and job markets might play a role in attracting different genders to specific regions.



# Sughra

4. In which year did immigrants, non-immigrants, and non-permanent residents reach their highest numbers?

