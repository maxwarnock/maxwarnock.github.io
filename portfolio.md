---
layout: default
title: Portfolio
show_profile: false
---

# Portfolio
---
**Annual Temperatures in Aspen Increasing by 0.0061 °C per year on Average Since 1980**   
10/1/25

Aspen Colorado is a popular destination for winter sports of all kinds. It's known for its pristine powder which is great for skiing and snowboarding. Since the economy of Aspen is so dependent on low winter temperatures and good snow conditions, I wanted to determine if there have been any trends in Aspen's climate over the last several decades.  
<img src="img/Maroon_Bells.jpg" alt="Maroon Bells" width="400">   
*Photo credit: https://commons.wikimedia.org/wiki/User:Rhododendrites*   
To research this, I searched for weather station data in Aspen available from the [Global Historical Climatology Network daily (GHCNd)](https://www.ncdc.noaa.gov/cdo-web/datasets), provided by NOAA's [National Centers for Environmental Information (NCEI)](https://www.ncei.noaa.gov/access). I used station ASPEN 1 SW, CO US, which has 99% daily temperature summary data coverage from 1980 to present. According to [NASA](https://science.nasa.gov/climate-change/what-is-climate-change/), a 30 year timespan is required to observe any meaningful change in climate, while timespans less than this simply show variability in weather patterns. The station I chose has a 45 year timespan of consistent data coverage, meaning that this timespan is long enough to observe meaningful changes in climate. 


<embed type="text/html" src="/img/aspen_temp_interactive.html" width="720" height="320"> 
This graph shows an increase in average annual temperature in Aspen, CO of 0.0061 °C per year since 1980. Over 45 years, this is an increase of 0.2745 °C. 



[View my full workflow](./img/Aspen_Climate_data.html){:target="_blank"}

Considerations for using Linear Ordinary Least Squares (OLS) Regression

- Random error: With OLS, we are assuming that all temperature variation except for climate change is random. However, El Nino and La Nina can be predicted to a certain extent, and so this is a certain amount of variation that is not random that OLS is not considering. However, there is still a lot of weather variability that is random.
- Normally Distributed Error: This data is a good application in terms of normally distributed error because we are looking at average annual temperature, and not something like daily precipitation or temperature. 
- Linearity: By looking at the data of temperature gradually increasing over time, it appears you could draw a straight line through it. It does not appear curved or exponential, so in this case, this looks like a good reason to use OLS. 
- Stationarity: The amount of variability (randomness) over time appears roughly the same across the timespan. There are some areas with more or less variability, but across the entire 120 years, there is no meaningful shift in randomness, so this is a good reason to use OLS.

---
**Creating html maps using OpenStreetMaps**   
9/10/25
<embed type="text/html" src="/img/glacier.html" width="600" height="485">
A few years ago, I worked on a project using satellite imagery to measure the size of glaciers in Grand Teton National Park over time. My findings showed that the glaciers were rapidly losing size over just a 20 year timeframe. This map shows the general location of the some of the glaciers I studied. 

