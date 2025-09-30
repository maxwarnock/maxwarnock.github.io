---
layout: default
title: Portfolio
show_profile: false
---

# Portfolio
---
9/24/25 - Boulder Climate Change plot
<embed type="text/html" src="/img/boulder_temp_plot.html" width="720" height="320">
**Annual Average Temperatures in Boulder Increasing by 2.172 °C Over Past 120 Years**   
This graph shows an increase in average temperature in Boulder over time, meaning that the climate is changing. The slope of the trendline is 0.0181 °C per year. Over 120 years, this is a 2.172 °C increase which is very significant and concerning.   

Considerations for using Linear Ordinary Least Squares (OLS) Regression

- Random error: With OLS, we are assuming that all temperature variation except for climate change is random. However, El Nino and La Nina can be predicted to a certain extent, and so this is a certain amount of variation that is not random that OLS is not considering. However, there is still a lot of weather variability that is random.
- Normally Distributed Error: This data is a good application in terms of normally distributed error because we are looking at average annual temperature, and not something like daily precipitation or temperature. 
- Linearity: By looking at the data of temperature gradually increasing over time, it appears you could draw a straight line through it. It does not appear curved or exponential, so in this case, this looks like a good reason to use OLS. 
- Stationarity: The amount of variability (randomness) over time appears roughly the same across the timespan. There are some areas with more or less variability, but across the entire 120 years, there is no meaningful shift in randomness, so this is a good reason to use OLS.

---
9/10/25 - Creating html maps
<embed type="text/html" src="/img/glacier.html" width="600" height="485">
A few years ago, I worked on a project using satellite imagery to measure the size of glaciers in Grand Teton National Park over time. My findings showed that the glaciers were rapidly losing size over just a 20 year timeframe. This map shows the general location of the some of the glaciers I studied. 

