## Study of Annual Migration Patterns of the Baltimore Oriole (Icterus galbula)
10/29/25  

<a href="https://maxwarnock.github.io/projects/oriole-migration/baltimore-oriole-migration-notebook" target="_blank" rel="noopener noreferrer" style="font-weight: bold;">Link to my complete analysis and Python code</a><br>
<a href="https://github.com/maxwarnock/Baltimore_Oriole_Migration/tree/main" target="_blank" rel="noopener noreferrer" style="font-weight: bold;">Link to my GitHub repository</a>

<p align="justify">
  <img src="https://maxwarnock.github.io/img/baltimore-oriole-image.jpg" alt="Baltimore Oriole" align="left" width="250" style="margin-right: 10px; margin-bottom: 3px;">
<strong>Introduction</strong><br>   
  The Baltimore Oriole (Icterus galbula) is a colorful migratory bird found throughout the Eastern/Central part of North and Central America. The male has bright orange and black plumage which makes it easy to spot, while the female plumage is only slightly less brilliant. Like many species, the Baltimore Oriole spends the winters in the warmer climates of Central America, and migrates north during the summer (<a href="https://www.allaboutbirds.org/guide/Baltimore_Oriole/overview"
    target="_blank"
    rel="noopener noreferrer">Cornell Lab of Ornithology</a>). According to the <a href="https://www.audubon.org/field-guide/bird/baltimore-oriole">Audubon Society</a>, Orioles prefer open woods, riverside groves, elms, and shade trees, and generally prefer to nest on the edges of woodlands. The Audubon Society also notes that this species still has a healthy population, but "surveys show a decline in recent decades." In particular, Dutch elm disease during the mid 20th century may have contributed to a loss of habitat for Orioles. Climate change is another factor threatening Orioles. The Audubon Society lists fire weather, spring heat waves, and urbanization as leading climate change related factors that are negatively impacting Oriole populations.
</p>


**Migration Mapping**   
Knowing the month-by-month range of the Baltimore Oriole's migration path can be a useful tool for conservation efforts. Since the Oriole is a migratory species, it relies on a wide range of habitats across Central and North America. Knowing when and where this species will be can aid conservation efforts. While this analysis focuses on the 2024 migration range, mapping the range over multiple years or decades can be an important way of assessing the health of the Oriole population.

**Migration Data from GBIF**    
To map the Oriole's annual migration, I will be using occurrence data from the [Global
Biodiversity Information Facility (GBIF)](https://www.gbif.org/). Occurrence data is largely collected using [eBird](https://ebird.org/home) and [iNaturalist](https://www.inaturalist.org/), as well as several other reputable citizen science data sources ([GBIF Data Processing](https://www.gbif.org/data-processing)).

**Ecoregion Data**   
I will be plotting occurrence (sightings of Orioles) data within ecoregions to visualize the Oriole migration on a map. For the ecoregion data, I will be using data published in 2017 by [RESOLVE](https://www.resolve.ngo/) and [OneEarth](https://www.oneearth.org/announcing-the-release-of-ecoregion-snapshots/).  

**Data Processing**   
After downloading the data, there are several steps necessary to plot the data geographically over time. Major steps included joining both datasets, counting observations in each ecoregion per month, and normalizing for space and time. 

**Normalization**   
The goal of this analysis is not only to plot geographically, but to also represent density of bird observations using a color gradient. The goal of the normalization step is to remove systematic differences such as some months have more sampling because more birdwatchers are outside, and some regions being more heavily surveyed because more birdwatchers live there.
  
<embed type="text/html" src="https://maxwarnock.github.io/projects/oriole-migration/baltimore-oriole-migration.html" width="800" height="650">

**Figure 1:** Interactive map of the Baltimore Oriole's 2024 migration using GBIF occurrence data. Each ecoregion is shaded by its normalized occurrence value for the selected month, with darker blue representing a higher density of Oriole observations after accounting for ecoregion size and sampling effort. Ecoregions with fewer than two observations in a month are not shown. Use the slider below the map to step through the months. See my <a href="https://maxwarnock.github.io/projects/oriole-migration/baltimore-oriole-migration-notebook" target="_blank" rel="noopener noreferrer">complete analysis</a> for a full explanation of the normalization steps.

**Results and Analysis**   
According to the interactive plot above, the Baltimore Oriole spends the coldest winter months (December/January) in warmer climates with ecoregions with dense observations in South and Central America. Surprisingly, there are also less dense ecoregions with Orioles along the East Coast of North America, extending into Canada during the coldest months. This suggests that while Orioles may prefer the warmer climates of the South, they can still tolerate the colder winter weather along the East Coast. There are also observations of Orioles on the Caribbean islands in most months except for summer, suggesting that Orioles are very capable of migrating across fairly large water bodies. 

During the summer months, Orioles are almost solely observed in the U.S. and Canada, and are almost completely absent from their winter habitats in Central and South America. Additionally, the Oriole's range appears to be limited by the geographic barrier of the Rocky Mountains. This might be explained by the Oriole's habitat preferences which don't align well with the dense forests and steep terrain of the Rockies. However, the Oriole is not afraid to venture far north, with ecoregions with very dense summer observations found in the Northern U.S. and Canada. 

These results align closely with maps and information provided by the [Cornell Lab of Ornithology](https://www.allaboutbirds.org/guide/Baltimore_Oriole/overview) and the [Audubon Society](https://www.audubon.org/field-guide/bird/baltimore-oriole). 


**Conclusion**    
The goal of this analysis was to map the month-by-month range of the Baltimore Oriole's 2024 migration using GBIF occurrence data summarized by ecoregion. After normalizing the observations for ecoregion size and for differences in sampling effort across months and regions, the map shows a clear seasonal pattern. Orioles spend the winter mostly in Central and South America and the Caribbean, with smaller numbers staying along the East Coast of North America. In the summer, they move north into the Eastern and Central U.S. and Canada, staying mostly east of the Rocky Mountains. These results are consistent with the range maps and descriptions from the [Cornell Lab of Ornithology](https://www.allaboutbirds.org/guide/Baltimore_Oriole/overview) and the [Audubon Society](https://www.audubon.org/field-guide/bird/baltimore-oriole), which suggests that citizen science data from GBIF can be a useful tool for tracking bird migration. However, this analysis only covers a single year, and even after normalization the data still reflects where people are out birdwatching. Repeating this analysis over multiple years or decades would help show whether the Oriole's range is shifting in response to the habitat loss and climate change threats described by the Audubon Society.


**Works Cited**    
Cornell Lab of Ornithology. Baltimore Oriole Overview. All About Birds. <https://www.allaboutbirds.org/guide/Baltimore_Oriole/overview>

Dinerstein, E., Olson, D., Joshi, A., Vynne, C., Burgess, N.D., Wikramanayake, E., et al. (2017). An Ecoregion-Based Approach to Protecting Half the Terrestrial Realm. BioScience, 67(6), 534–545. <https://doi.org/10.1093/biosci/bix014>

ESIIL Learning Portal. Mapping migration. Earth Data Analytics Textbook. <https://earthdatascience.org/notebooks/03-migration/migration-eda.html>

GBIF. Data processing. Global Biodiversity Information Facility. <https://www.gbif.org/data-processing>

GBIF.org. Icterus galbula (Baltimore Oriole) occurrence data, 2024. Global Biodiversity Information Facility. <https://www.gbif.org/species/2484340>

National Audubon Society. Baltimore Oriole. Audubon Field Guide. <https://www.audubon.org/field-guide/bird/baltimore-oriole>

One Earth. Announcing the release of Ecoregion Snapshots. <https://www.oneearth.org/announcing-the-release-of-ecoregion-snapshots/>

*Photo: Baltimore Oriole. Source: [AllAboutBirds.org](https://www.allaboutbirds.org/guide/assets/og/615439951-1200px.jpg)*
