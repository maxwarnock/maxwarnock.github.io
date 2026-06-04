## Analysis of the Migration Range of the American Redstart (Setophaga ruticilla) from 2004 to 2024 {#redstart}
12/10/25

**[Link to my complete analysis, Python code, and repository](https://maxwarnock.github.io/projects/redstart-migration/migration_download_steps)**

<p align="justify">
  <img src="https://www.allaboutbirds.org/guide/assets/og/75237001-1200px.jpg" alt="Redstart" align="right" width="350" style="margin-left: 10px; margin-bottom: 3px;">
<strong>Introduction</strong><br> 
  The American Redstart (Setophaga ruticilla) is a colorful warbler that migrates across the Americas each year. Males have a dark black head and chest, with bright orange on the wings, sides, and tail, while females are a lighter grey color with yellow highlights. These warblers prefer nesting in open woodlands across North America <a href="https://www.allaboutbirds.org/guide/American_Redstart/overview"
    target="_blank"
    rel="noopener noreferrer">(Cornell Lab of Ornithology)</a>. They spend the winters in Central and South America, and migrate as far as Northern Canada for breeding during the summer. Like many migratory birds, climate change and human developments are impacting the Redstart's migration patterns and survival according to the (<a href="https://www.caryinstitute.org/news-insights/feature/climate-change-pushing-american-redstarts-breeding-range-southward"
    target="_blank"
    rel="noopener noreferrer">Cary Institute of Ecosystem Studies</a>).
</p>

**Research Question**    
Is there an identifiable change or trend in the extent of the American Redstart's total annual range from 2004 to 2024? 

**Migration Patterns, Climate Change, and Deforestation**    
American Redstarts are being affected by climate change in some parts of their migration range. According to Bryant Dossman, a conservation and migration ecology scientist, Redstarts are particularly affected by increasingly dry conditions in the tropics of South America and Jamaica where many Redstarts spend the winter [(Heisman, 2024)](https://www.allaboutbirds.org/news/american-redstarts-can-speed-up-their-migration-but-theres-a-cost/). There is strong evidence that increasingly dry conditions in the tropics are linked to climate change and deforestation [(Y. Malhi, et al)](https://royalsocietypublishing.org/rstb/article-abstract/359/1443/331/20382/Tropical-forests-and-the-global-carbon-cycle?redirectedFrom=fulltext) and [(Franco. M.A, et al)](https://doi.org/10.1038/s41467-025-63156-0). According to Dossman, these conditions are making it harder for the Redstart to find enough food and insects to put on enough weight for the migration journey north. Dossman observes that this causes the Redstart to often leave later in the spring. Dossman used GPS tracking devices on the birds to study their migration speed. He found that bird that left late migrated faster to make up for lost time. However, he notes that migrating faster increases stress and energy expenditure of the birds, making them more likely to die on the journey. Dossman found that birds that left late had a 6% increased risk of death on their migration journey as opposed to birds that left on time [(Heisman, 2024)](https://www.allaboutbirds.org/news/american-redstarts-can-speed-up-their-migration-but-theres-a-cost/). Another similar study from 2015 found very similar results to Dossman [(Cooper, N.W, et al)](https://doi.org/10.1890/14-1365.1). 

These studies indicate that an increasing lack of resources in South America is impacting the Redstart's range. According to the Cary Institute of Ecosystem Studies, the Redstart is migrating farther south into South America during the winters in search of food, and not as far north into Canada during the summers because of the delay migrating north. The overall effect is that the Redstart's range is shifting southwards [(Cary Institute of Ecosystem Studies)](https://www.caryinstitute.org/news-insights/feature/climate-change-pushing-american-redstarts-breeding-range-southward).


**Migration Mapping**    
Because of the impacts described above, knowing the month-by-month range of the Redstart's migration path can be a useful tool for conservation efforts. In addition to the month-by-month range, assessing the range over years and decades can confirm important information about how climate change and deforestation is impacting the Redstart's range. 


**Migration Data from GBIF**    
To map the Redstart's annual migration, I will be using occurrence data from the [Global Biodiversity Information Facility (GBIF)](https://www.gbif.org/). Occurrence data is largely collected using [eBird](https://ebird.org/home) and [iNaturalist](https://www.inaturalist.org/), as well as several other reputable citizen science data sources [(GBIF Data Processing)](https://www.gbif.org/data-processing).

**Ecoregion Data**    
I will be plotting occurrence (sightings of Redstarts) data within ecoregions to visualize the Redstart migration on a map. For the ecoregion data, I will be using data published in 2017 by [RESOLVE](https://www.resolve.ngo/) and [OneEarth](https://www.oneearth.org/announcing-the-release-of-ecoregion-snapshots/).

**Results**

<div style="
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
">
  <iframe src="https://maxwarnock.github.io/img/redstart-migration-2004.html" style="width: 100%; height: 370px; border:none;"></iframe>
  <iframe src="https://maxwarnock.github.io/img/redstart-migration-2009.html" style="width: 100%; height: 370px; border:none;"></iframe>
  <iframe src="https://maxwarnock.github.io/img/redstart-migration-2014.html" style="width: 100%; height: 370px; border:none;"></iframe>
  <iframe src="https://maxwarnock.github.io/img/redstart-migration-2019.html" style="width: 100%; height: 370px; border:none;"></iframe>
</div>

**Figure 1:** Maps showing the month-by-month migration patterns of the American Redstart for years 2004, 2009, 2014, 2019. Density of observations is represented by the blue color scale. 

<embed type="text/html" src="https://maxwarnock.github.io/img/redstart-migration-years.html" width="800" height="650">

**Figure 2:** Map showing the entire range of the American Redstart for the years of 2004, 2009, 2014, 2019, and 2024. Density of observations for the entire year is represented by the blue color scale. Yearly density values were calculated by taking the sum of monthly normalized occurrence values. See my download-200X.ipynb files in my repository for a full explaination of normalization steps.

**Analysis**    
The map above shows the entire migration range of the Redstart for the years of 2004, 2009, 2014, 2019, and 2024. In 2004, notice the northern extent of the Redstart in Northwestern Canada. This ecoregion disappears in later years, meaning the Redstart has not been observed in that northern ecoregion in more than a decade according to the GBIF data. As you scroll through the years, also notice the range extent in South America. In 2004, the range is fairly limited in South America. However, the Redstart's range in South America has gradually been increasing southward, as well as the density of observations. Notice that the density of observations in 2004 is relatively low. However, in more recent years, the density is much higher. 


**Conclusion**    
According to the [Cornell Lab of Ornithology](https://www.allaboutbirds.org/guide/American_Redstart/overview), the [Cary Institute of Ecosystem Studies](https://www.caryinstitute.org/news-insights/feature/climate-change-pushing-american-redstarts-breeding-range-southward), and the study by [Cooper et al](https://doi.org/10.1890/14-1365.1), the American Redstart's migration range has been forced southwards in recent decades due to climate change impacts on their habitat, particularly in Central and South America. This analysis focused on two decades of data of GBIF observations of the Redstart's range in order to observe trends in the extent of the Redstart's range. The resulting map shows an increase in the extent of the Redstart's southern range during the winter months, indicating that the bird is venturing farther into South America in search of food. Additionally, the Northern range reduced slightly. These findings are consistent with the studies cited above, showing that the Redstart's range is being affected by climate change and deforestation. While the species appears to be adapting and its population is stable, these affects are putting an increased strain on its migration patterns and could lead to more negative impacts in the future if conditions worsen [(Heisman, 2024)](https://www.allaboutbirds.org/news/american-redstarts-can-speed-up-their-migration-but-theres-a-cost/).


**Works Cited**    
Cary Institute of Ecosystem Studies. Climate change is pushing the American redstart’s breeding range southward. https://www.caryinstitute.org/news-insights/feature/climate-change-pushing-american-redstarts-breeding-range-southward

Cooper, N.W., Sherry, T.W. and Marra, P.P. (2015), Experimental reduction of winter food decreases body condition and delays migration in a long-distance migratory bird. Ecology, 96: 1933-1942. https://doi.org/10.1890/14-1365.1 

Cornell Lab of Ornithology. American Redstart. https://www.allaboutbirds.org/guide/American_Redstart/overview 

Franco, M.A., Rizzo, L.V., Teixeira, M.J. et al. How climate change and deforestation interact in the transformation of the Amazon rainforest. Nat Commun 16, 7944 (2025). https://doi.org/10.1038/s41467-025-63156-0

Heisman, Rebecca. American Redstarts Can Speed Up Their Migration, but There’s a Cost. Cornell Lab of Ornithology. 2024. https://www.allaboutbirds.org/news/american-redstarts-can-speed-up-their-migration-but-theres-a-cost/.

Y. Malhi, O. L. Phillips, Wolfgang Cramer, Alberte Bondeau, Sibyll Schaphoff, Wolfgang Lucht, Benjamin Smith, Stephen Sitch; Tropical forests and the global carbon cycle: impacts of atmospheric carbon dioxide, climate change and rate of deforestation. Philos Trans R Soc Lond B Biol Sci 29 March 2004; 359 (1443): 331–343. https://doi.org/10.1098/rstb.2003.1428
