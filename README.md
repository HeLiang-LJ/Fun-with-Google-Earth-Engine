# geeFSN
 Google Earth Engine self-learning. Resources for myself.\
 Start from the official guide and the reference: https://developers.google.com/earth-engine/#api \
 Copy the script and run in the GEE code editor: https://code.earthengine.google.com/
## 1. [Mean Annual Temperature/PrecipitationNoah](https://github.com/fsn1995/geeFSN/blob/master/Noah.js)
This script computes, displays and exports the mean annual temperature, mean annual precipitation. The selected dateset is NOAH Global Land Assimulation System data.\
The temporal resolution is 3 hours (8 bands per day). Note: the unit of precipitation rate (kg/m^2/s) equals mm/s and is converted by the script. More about the data can be found at: \
https://developers.google.com/earth-engine/datasets/catalog/NASA_GLDAS_V20_NOAH_G025_T3H \
https://developers.google.com/earth-engine/datasets/catalog/NASA_GLDAS_V021_NOAH_G025_T3H \
![screenshot](pic/MAP.jpg)
![screenshot](pic/MAT/jpg)    
## 2. [GRACE](https://github.com/fsn1995/geeFSN/blob/master/grace.js)
This script displays the long term average GRACE (the Gravity Recovery and Climate Experiment) data.\
![screenshot](pic/grace.png)  
## 3. Visualization of Globa Product
This part aims to visualize some of the global product in the GEE's dataset. Some of the scripts were explored while I am working as the RS and GIS associate at the ICRC.
## 3.1 EC JRC/Google Global Product 
Explore the global surface product provided by EC JRC/Google. 
### 3.1.1 [Global Water](https://github.com/fsn1995/geeFSN/blob/master/GlobalWater.js)
It would display the global surface water dynamics in your area of interest. 
![screenshot](pic/globalwater.png)  
### 3.1.2 [Global Water Annual Time Slider](https://github.com/fsn1995/geeFSN/blob/master/GloablWaterAnnual.js)
It creates a dateslider to check the annual water classification. 
![screenshot](pic/annualwater.png)  
### 3.1.3 [Global Urban](https://github.com/fsn1995/geeFSN/blob/master/GlobalUrban.js)
This script utizes the GHSL: Global Human Settlement Layers, Built-Up Grid 1975-1990-2000-2015 (P2016) data.
![screenshot](pic/globalurban.png)  
### 3.2 [Fire Viewer](https://github.com/fsn1995/geeFSN/blob/master/FireViewer.js)
It displays the maximum extent of fire events during the study period at specified country. This was used to assist ICRC GIS officers from Lebanon to locate wildfires. The polygons of fire events can be exported via google drive.\
The data is provided by NASA / LANCE / EOSDIS (FIRMS: Fire Information for Resource Management System)
## 4. [koppen climate classification](https://github.com/fsn1995/geeFSN/blob/master/koppen.js)
This script displays The Köppen-Geiger climate map with a spatial resolution of 5 arc minutes for the period of 1986-2010. The legend will be displayed in the console.\
http://koeppen-geiger.vu-wien.ac.at/ \
Link to the shared data:\
https://code.earthengine.google.com/?asset=users/fsn1995/Global_19862010_KG_5m \
![screenshot](pic/koppen.png)  \
## 5. [Trend Analysis](https://github.com/fsn1995/geeFSN/blob/master/mannKendall.js)
This script performs Mann-kendall's test to the MODIS NDVI product. The result can be used to indicate the long-term trend of global vegetation (green) trend.\
![screenshot](pic/mannkendal.jpg)
# quick link
1) gee community: 
https://github.com/gee-community/
2) how to add a legend?
https://mygeoblog.com/2016/12/09/add-a-legend-to-to-your-gee-map/
3) how to add a gradient legend?
https://mygeoblog.com/2017/03/02/creating-a-gradient-legend/