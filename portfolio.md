---
layout: default
title: Portfolio
show_profile: false
---

# Portfolio
<hr style="height: 4px; background-color: black; border: none; margin: 20px 0;">

## Study of Annual Migration Patterns of the Baltimore Oriole (Icterus galbula)
10/29/25

**Introduction**   

<p align="justify">
  <img src="img/baltimore-oriole-image.jpg" alt="Baltimore Oriole" align="left" width="250" style="margin-right: 10px; margin-bottom: 3px;">
  The Baltimore Oriole (Icterus galbula) is a colorful migratory bird found throughout the Eastern/Central part of North and Central America. The male has bright orange and black plummage which makes it easy to spot, while the female plummage is only slightly less brilliant. Like many species, the Baltimore Oriole spends the winters in the warmer climates of Central American, and migrates north during the summer (<a href="https://www.allaboutbirds.org/guide/Baltimore_Oriole/overview"
    target="_blank"
    rel="noopener noreferrer">Cornell Lab of Ornithology</a>). According to the <a href="https://www.audubon.org/field-guide/bird/baltimore-oriole">Audubon Society</a>, Orioles prefer open woods, riverside groves, elms, and shade trees, and generally prefer to nest on the edges of woodlands. The Audubon Society also notes that this species still has a healthy population, but "surveys show a decline in recent decades." In particular, Dutch elm disease during the mid 20th century may have contributed to a loss of habitat for Orioles. Climate change is another factor threatening Orioles. The Audubon Society lists fire weather, spring heat waves, and urbanization as leading climate change related factors that are negatively impacting Oriole populations.
</p>


**Migration Mapping**   
Knowing the month-by-month range of the Balitmore Oriole's migration path can be a useful tool for conservation efforts. Since the Oriole is a migratory species, it relies on a wide range of habitats across Central and North America. Knowing when and where this species will be can aid conservation efforts. While this analysis focuses on the 2024 migration range, mapping the range over multiple years or decades can be an important way of assessing the health of the Oriole population.

**Migration Data from GBIF**   
To map the Oriole's annual migration, I will be using occurrence data from the [Global
Biodiversity Information Facility (GBIF)](https://www.gbif.org/). Occurrence data is largely collected using [eBird](https://ebird.org/home) and [iNaturalist](https://www.inaturalist.org/), as well as several other reputable citizen science data sources ([GBIF Data Processing](https://www.gbif.org/data-processing)).

**Ecoregion Data**   
I will be plotting occurrence (sightings of Orioles) data within ecoregions to visualize the Oriole migration on a map. For the ecoregion data, I will be using data published in 2017 by [RESOLVE](https://www.resolve.ngo/) and [OneEarth](https://www.oneearth.org/announcing-the-release-of-ecoregion-snapshots/).  

**Data Processing**   
After downloading the data, there are several steps necessary to plot the data geographically over time. Major steps included joining both datasets, counting observations in each ecoregion per month, and normalizing for space and time. 

**Normalization**   
The goal of this analysis is not only to plot geographically, but to also represent density of bird observations using a color gradient. The goal of the normalization step is to remove systematic differences such as some months have more sampling because more birdwatchers are outside, and some regions being more heavily surveyed because more birdwatchers live there.

[Click here to view my full analysis and Python code](./img/baltimore-oriole-migration-notebook)

<a href="./img/baltimore-oriole-migration-notebook" target="_blank" rel="noopener noreferrer">Click here to view my full analysis and Python code</a>

  
<embed type="text/html" src="/img/baltimore-oriole-migration.html" width="800" height="650">

**Results and Analysis**   
According to the interative plot above, the Baltimore Oriole spends the coldest winter months (December/January) in warmer climates with ecoregions with dense observations in South and Central America. Surprisingly, there are also less dense ecoregions with Orioles along the East Coast of North America, extending into Canada during the coldest months. This suggests that while Orioles may prefer the warmer climates of the South, they can still tolorate the colder winter weather along the East Coast. There are also observations of Orioles on the Carribean islands in most months except for summer, suggesting that Orioles are very capable of migrating across fairly large water bodies. 

During the summer months, Orioles are almost solely observed in the U.S. and Canada, and are almost completely absent from their winter habitats in Central and South America. Additionally, the Orioles range appears to be limited by the geographic barrier of the Rocky Mountains. This might be explained by the Oriole's habitat preferences which don't align well with the dense forests and steep terrain of the Rockies. However, the Oriole is not affraid to venture far north, with ecoregions with very dense summer observations found in the Northern U.S. and Canada. 

These results align closely with maps and information provided by the [Cornell Lab of Ornithology](https://www.allaboutbirds.org/guide/Baltimore_Oriole/overview) and the [Audubon Society](https://www.audubon.org/field-guide/bird/baltimore-oriole). 


<hr style="height: 4px; background-color: black; border: none; margin: 20px 0;">

## Annual Temperatures in Aspen Increasing by 0.0061 °C per year on Average Since 1980 
10/1/25

**Introduction**   
Aspen Colorado is a popular destination for winter sports, known for its pristine powder which is great for skiing and snowboarding. Since the economy of Aspen is so dependent on low winter temperatures and good snow conditions, I wanted to determine if there have been any trends in Aspen's climate over the last several decades.  
<img src="img/Maroon_Bells.jpg" alt="Maroon Bells" width="400">   
*Photo credit: https://commons.wikimedia.org/wiki/User:Rhododendrites*   
To research this, I searched for weather station data in Aspen available from the [Global Historical Climatology Network daily (GHCNd)](https://www.ncdc.noaa.gov/cdo-web/datasets), provided by NOAA's [National Centers for Environmental Information (NCEI)](https://www.ncei.noaa.gov/access). I used station ASPEN 1 SW, CO US, which has 99% daily temperature summary data coverage from 1980 to present. According to [NASA](https://science.nasa.gov/climate-change/what-is-climate-change/), a 30 year timespan is required to observe any meaningful change in climate, while timespans less than this simply show variability in weather patterns. The station I chose has a 45 year timespan of consistent data coverage, meaning that this timespan is long enough to observe meaningful changes in climate. 

The raw data has daily average temperatures, and I wanted annual average temperature values to understand longer term changes in climate. In Python, I calculated the annual mean values and resampled to one temperature value per year. Next, I used the sklearn library to fit a trendline to the data using the Linear Ordinary Least Squares (OLS) Regression method.

<embed type="text/html" src="/img/aspen_temp_interactive.html" width="720" height="320"> 
This graph shows an increase in average annual temperature in Aspen, CO of 0.0061 °C per year since 1980. Over 45 years, this is a total increase of 0.2745 °C.   

[View my Python workflow](./img/Aspen_Climate_data.html){:target="_blank"}

<hr style="height: 4px; background-color: black; border: none; margin: 20px 0;">

## Creating html maps using OpenStreetMaps  
9/10/25
<embed type="text/html" src="/img/glacier.html" width="600" height="485">
A few years ago, I worked on a project using satellite imagery to measure the size of glaciers in Grand Teton National Park over time. My findings showed that the glaciers were rapidly losing size over just a 20 year timeframe. This map shows the general location of the some of the glaciers I studied. 

