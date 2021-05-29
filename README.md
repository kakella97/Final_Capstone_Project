# Final_Capstone_Project
## Analysis of BC's Lower Mainland Venue and Housing Data

### Introduction/Business Problem and Data:
#### Intro: 
British Columbia (BC) contains some of the most expensive housing markets not only in Canada but all of North America. The buying craze may stem from a high demand along with a scarce supply, low interest rates and a financially strong middle class. In addition, cities like Vancouver have become extremely desirable to live in, which in turn increases the demand with limited supply. Due to these reasons, it has become the most expensive city in BC. Of course there are many possible explanations and I intend on discovering some of these answers from this project.

#### Business Problem and Target Audience: 
The objective of this project is to understand the connection between common venues and housing prices in the lower mainland of BC. This problem may interest investors looking to start new businesses where real estate costs are low but demand for a certain type of venue is high. Additionally, home buyers may want to know what cities have the least expensive housing prices, the different social locations, and options for transit. Likewise, realtors may use this information to help someone buy a house.

#### Data:
The data will consist of average housing prices per area, area, neighborhood, latitude and longitude of each neighborhood. The latitude and longitude data can be extracted via the GeoPy library since I have the neighborhood and area data. I will webscrape this site for the average housing prices per area, area, neighborhood data: https://www.moneysense.ca/spend/real-estate/where-to-buy-real-estate-in-2020-greater-vancouver/. I will then use the Foursquare API to get venue data for each neighborhood using the longitude and latitude information gained earlier. The venue data may consist of any type of venue. I will attempt to extract venue data with a radius of 500 and a limit of 100. I will then use a geoJSON file to get geospatial data on each area so that I can create a choropleth map showing different housing prices in each area. I will get the geoJSON file from here: https://catalogue.data.gov.bc.ca/dataset/municipalities-legally-defined-administrative-areas-of-bc#edc-pow. 
