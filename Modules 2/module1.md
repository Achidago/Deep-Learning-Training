# Module 1 - Time Series Analysis 


**What will you learn from this module?**
- Time Series Analysis Concept and fundamentals
- Time Series Analysis Methods
- Techniques for Time Series Analysis in GEE

## 1. Introduction to Time Series Analysis
**Time series analysis** looks at landscape change as a dynamic process over several months, years, etc. Mapping the environment at various timescales can provide information about land monitoring parameters like land cover change trends and patterns in vegetation growth. Time series of satellite observations are used to derive environmental parameters to evaluate environmental conditions. <br>

**Common Applications of Time Series Analysis:**
- Identifying urban expansion
- Land cover changes
- Mapping deforestation
- Monitoring post-fire conditions

<p align="center">
<img src="https://user-images.githubusercontent.com/85199074/194786938-24b992c2-f1b2-4972-97b5-5a0ba0b7633a.jpg">
</p>
<sub> Landcover changes for Greater Accra Metropolitan Area (GAMA) from the year 1991 to 2015.</sub>

([Source](https://www.mdpi.com/2413-8851/3/1/26))<br>


## 2. Basics of Time Series Analysis
- **Spatial/geospatial data** is information about locations and shapes of objects in a geographic coordinate system and is represented as shapes in the form of points, paths and surfaces. <br>
- **Temporal data** is data that represents a state in time. <br>
- **Spatio-temporal** databases host data collected across both space and time that describe a phenomenon in a particular location and period of time. 

<p align="center">
<img src="https://user-images.githubusercontent.com/87503837/151854688-12a69e04-c870-4273-88e6-4c30e7b9d7d5.png">
</p>

([Source](https://doi.org/10.1186/s40965-017-0038-z))<br>
MODIS NDVI and EVI

**Imagery Selection Guide:**
- Images should be selected at particular times aand seasons depending on the application. For istance phenological differences or Land cover chnages.
- Seasonal trends result from differences in precipitation and temperature.
- Be aware of different annual weather conditions – For example, drought years vs. non-drought years.

**Types of Time Series Analysis**
- **Annual Trends:**
It is a yearly assessment undertaken for as many years as possible (availability of data). It is particularly useful for land use/land cover analysis over long periods of time.

<p align="center">
<img src="https://www.mdpi.com/land/land-09-00300/article_deploy/html/images/land-09-00300-g003.png">
</p>
<sub> Maps showing land cover change (LCC) characteristics in Kumasi (1986–2018)a. </sub>

([Source](https://www.mdpi.com/2073-445X/9/9/300/htm))<br>

- **Seasonal Trends:**
It is driven by annual temperature and/or precipitation to assess variation between seasons. It can measure change within a year timeframe and is useful in comparison of seasonal variation between years.

<p align="center">
<img src="https://media.springernature.com/lw685/springer-static/image/art%3A10.1007%2Fs12665-022-10481-y/MediaObjects/12665_2022_10481_Fig9_HTML.png?as=webp">
</p>
<sub> Temperature analysis over the study period (1970–2020) in Southwestern Ghana </sub>

([Source](https://link.springer.com/article/10.1007/s12665-022-10481-y))<br>

## 3. Methods of Time Series Analysis
- ##Yet to be devloped##
 
## 4. Time Series Analysis in GEE

GEE has a variety of functions useful for time series analysis:
- Filtering and compilation of data across large datasets over time. Refer to ([GALUP Training Module 2- Introduction to GEE](https://github.com/SERVIR-WA/GALUP/blob/master/training/2_rs/module2.md))<br>
- Analysis using map visualizations and user interface generated charts and graphs
<p align="center">
<img src="https://developers.google.com/static/earth-engine/images/Charts_image_collection_05.svg">
</p>
<sub> Example chart of time series NDVI data from MODIS plotted in GEE from 2010 to 2019. </sub>

([Source](https://developers.google.com/earth-engine/guides/charts_image_collection))<br>

**4.1 Video tutorial for the section 3.1** <br>

**4.2 Running Time Series Analysis**<br>
- In the following example, we will use GEE to run a Time Series Analysis and print a chart to show results for a selected area in Ghana. Please use the video tutorial in **Section 4.1** to follow along.

- Copy the script [Time Series Analysis](https://github.com/ecodynlab/GALUP/wiki/Scripts#04_time_series_analysis) and paste into the GEE code editor. This is the same script that will be used in Exercise with slight alterations necessary to complete the Exercise.
- The script includes:<br>
  a. Defining variables for dates of interest: **ST_DATE** and **EN_DATE** <br>
  b. Defining the region of interest using 4 coordinates: **Longitude_min**, **Latitude_min**, **Longitude_max**, **Latitude_max** or draw using drawing tools <br>
  c. Filtering the data product by the **region** and **dates of interest**. <br>
  d. Creating a function to add an **NDVI** band to an image collection. <br>
  e. Display the result. <br>
  f. Define the **chart** and **print**. <br>
   

## 5. Exercises and Post-training Survey

- Please complete the [Exercise 1]
- Please complete the [Exercise 2]

- Please take this [post-training survey]
  
- Please submit your exercises [here]

## 6. What's Next?

Module 2 - Landcover Change Detection

## 7. Other Useful Resources
 1. [Cloud-Based Remote Sensing with Google Earth Engine](https://www.eefabook.org/go-to-the-book.html)<br>
 2. [NASA ARSET: Time Series Analysis](https://www.youtube.com/watch?v=RqVselZ5hKM&t=3695s)<br>