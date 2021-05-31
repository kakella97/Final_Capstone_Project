# Final_Capstone_Project
## Analysis of BC's Lower Mainland Venue and Housing Data

### Introduction/Business Problem and Data:
#### Intro: 
British Columbia (BC) contains some of the most expensive housing markets not only in Canada but all of North America. The buying craze may stem from a high demand along with a scarce supply, low interest rates and a financially strong middle class. In addition, cities like Vancouver have become extremely desirable to live in, which in turn increases the demand with limited supply. Due to these reasons, it has become the most expensive city in BC. Of course there are many possible explanations and I intend on discovering some of these answers from this project.

#### Business Problem and Target Audience: 
The OBJECTIVE of this project is to understand the connection between common venues and housing prices of cities in the lower mainland of BC. This problem may INTEREST investors looking to start new businesses where real estate costs are low but demand for a certain type of venue is high. Additionally, home buyers may want to know what cities have the least expensive housing prices, the different social locations, and options for transit. Likewise, realtors may use this information to help someone buy a house.

#### Data:
The data will consist of average housing prices per area, area, neighborhood, latitude and longitude of each neighborhood. The latitude and longitude data can be extracted via the GeoPy library since I have the neighborhood and area data. I will webscrape this site for the average housing prices per area, area, neighborhood data: https://www.moneysense.ca/spend/real-estate/where-to-buy-real-estate-in-2020-greater-vancouver/. I will then use the Foursquare API to get venue data for each neighborhood using the longitude and latitude information gained earlier. The venue data may consist of any type of venue. I will attempt to extract venue data with a radius of 500 and a limit of 100. I will then use a geoJSON file to get geospatial data on each area so that I can create a choropleth map showing different housing prices in each area. I will get the geoJSON file from here: https://catalogue.data.gov.bc.ca/dataset/municipalities-legally-defined-administrative-areas-of-bc#edc-pow. 

![Screenshot (92)](https://user-images.githubusercontent.com/51190520/120247269-c46e2d00-c227-11eb-928e-4c693e41a1c0.png)

As one can observe from the example above the foursquare API will give data about common venues for each neighborhood. This data will be converted from categorial data into numerical data which will be used in the K-Means clustering algorithm to find common venues. I will superimpose these clusters onto a choropleth map describing the different housing prices of different areas in BC. Please view the second example of the the housing price data below.

![image](https://user-images.githubusercontent.com/51190520/120247461-5d04ad00-c228-11eb-9920-1cb7b3ce5d34.png)

