# An analysis of the 3D shape of cities with respect to Urban Heat Island effect

# Abstract

The aim of this study was to explore how building shapes interact with urban policies and regulations. We plan to develop urban planning strategies aimed at mitigating Urban Heat Island effect as well as the impacts of, climate change to urban areas. We explore the relationship between variables like urban morphology, building heights, vegetation, green distribution, shadow and the UHI effect/ climate change (H M Abdul Fattah, 2024, p2)
Research has shown that urban areas tend to have higher temperatures compared to the surrounding rural areas. This effect is known as the urban heat island (UHI) [1].  The temperature increase within urban areas is known to lead to various problems including human health issues, increase in energy consumption thereby increasing greenhouse gas emissions, as well as further contributions to climate change. To reduce these effects there is need to identify factors related to UHI and take appropriate actions to mitigate its effect in urban areas.
Work done by Mr. H M Abdul Fattah on this project [8] consisted of downloading city shape file, building height dataset, calculating city wise area vs building height distribution and classifying cities into one of the four categories. Dataset about the heights of buildings globally (GHS-BUILT-H - R2023A) was obtai ned from  GHSL - Global Human Settlement Layer dataset[13] .  Additionally, shapefiles, defining urban areas , were obtained from World Urban Areas, LandScan, 1:10 million (2012) [14] . Data of heights of buildings was filtered using shape files and analysed to find the distribution of building heights in the city. Based on the shapes of distribution (their skewness and dip statistic values), the shape of city was classified as unimodal right skew  (Pyramid) shape, unimodal left skew (Inverse Pyramid) shape, or has no significant skew (Diamond) shape [15] [8]. In case of presence of multimodality, indicated by the dip statistic, shape was classified as  "Hourglass." The "Pyramid" class signifies a concentration of shorter buildings, while "Inverse Pyramid" indicates a concentration of taller buildings. "Diamond" suggests a balanced distribution of building heights, while "Hourglass" implies varying patterns in building height distribution.


# Introduction

Urban Heat Island (UHI) leads to increased vulnerability to human health issues like heat strokes, exhaustion, suicidal tendancies. It is also impacting air quality due to more amount of pollutants released in air and poor scattering of these pollutants. Water quality also gets impacted due to increase in water tempaerature affecting native aquatic life.[3]
 
Urban areas are densely populated with more people. Closely constructed building and skyscrapers mean a lot of waste energy is emitted and can not escape the area. Increase in temperature also causes increase in energy consumption thereby increasing greenhouse emissions  for the city dwellers. [2].
According to David L. Chandler, Urban heat island effects also depend on a city’s street and building layout Some cities, such as New York and Chicago, are laid out on a precise grid, like the atoms in a crystal, while others such as Boston or London are arranged more chaotically, like the disordered atoms in a liquid or glass. The researchers found that the “crystalline” cities had a far greater buildup of heat compared to their surroundings than did the “glass-like” ones.[4]
It is found that UHI is positively correlated with city area.  Building materials which absorb and radiate heat back into the air gets trapped in the nearby vicinity in the area densely crowded with buildings instead of spreading out evenly[5]. Hence effect of heights of skyscrapers also needs to be studied apart from the area of city. This can help in planning for urban area expansions or in new urban area developments

According to Nyuk Hien Wong, Chun Liang Tan, Dionysia Denia Kolokotsa & Hideki Takebayashi [6], 
Green infrastructure acts to cool the urban environment through shade provision and evapotranspiration. Typically, greenery on the ground reduces peak surface temperature by 2–9 °C, while green roofs and green walls reduce surface temperature by ~17 °C, also providing added thermal insulation for the building envelope. However, the cooling potential varies markedly, depending on the scale of interest (city or building level), greenery extent (park shape and size), plant selection and plant placement . This can be a tool for mitigating UHI 

Climate change is impacting cities and their residents in many ways, from poor air quality to flooding, biodiversity loss and extreme heat. Mackres et al.  [7] with the help of a dashboard provides insight into connection between climate change and urban life which will be useful for city designing in a more sustainable and nature-positive ways to mitigate climate change


Objective of this study is to determine the impact of building heights, city area expressed as city 3D shape on urban heat island effect observed in cities along with the impact of other variables like vegetation, water surfaces in the proximities of various cities spread across in the world

 
# Remarks

This repo has the following basic structure.

```
├── README.md           <- The top-level README for developers.
│
├── data            
│   ├── 01_raw          
│   ├── 02_intermediate 
│   ├── 03_processed    
│   ├── 04_models       
│   ├── 05_model_output 
│   └── 06_reporting   
│   └── 07_cities_shapefile      <- Shapefile of cities around the world
│   └── 08_cities_height         <- Building heights (raster data)
│   └── 09_continents_shapefile  <- Shapefile for continents
│   └── 10_raw_Other_variables   <- Downloaded raw data files 
│   └── 11_Output_R              <- Output files of R programs
│     └── city_rasters           <- Raster files generated using R programs
│   └── 12_Output_python         <- Output files of R programs
│
├── conf               
├── docs                <- Space for documentation. Can also included conceptualization and literature review.
│
├── references          <- Data dictionaries, manuals, reference manager (e.g. EndNote) etc.
│
├── results             
│   ├── submissions     
│
├── .gitignore          <- Avoids uploading data, credentials, outputs, system files etc.
│
├── src_py                    <- Python source code for use in this project.
│
├── src_r                     <- R source code for use in this project.
```

# References

[1] Urban heat island, Wikipedia, Available at https://en.wikipedia.org/wiki/Urban_heat_island
[2] Nidhi Singh, Saumya Singh, R.K. Mall. Urban ecology and human health: implications of urban heat island, air pollution and climate change nexus. Available at
https://www.sciencedirect.com/science/article/abs/pii/B9780128207307000173#:~:text=The%20UHI%20effect%20has%20caused%20an%20increase%20in,in%20nearby%20areas%20thus%20developing%20new%20ecological%20implications.  
[3] Urban Heat Island (nationalgeographic.org) Available at https://education.nationalgeographic.org/resource/urban-heat-island/ 
[4] David L. Chandler, Urban heat island effects depend on a city’s layout, Available at https://news.mit.edu/2018/urban-heat-island-effects-depend-city-layout-0222
[5] City module - City cluster and urban heat islands (Europe), Available at 
https://www.pik-potsdam.de/cigrasp-2/city-module/heat-island-cluster/index.html   
[6] Nyuk Hien Wong, Chun Liang Tan, Dionysia Denia Kolokotsa & Hideki Takebayashi Available at https://www.nature.com/articles/s43017-020-00129-5  
[7] Mackres, E., Pool, J. R., Shabou, S., Wong, T., Anderson, J., Gillespie, C., & Alexander, S. New Data Dashboard Helps Cities Build Urban Resilience in a Changing Climate. Available at
https://www.wri.org/update/new-data-dashboard-shows-climate-change-risks-in-cities  
[8] H. M. Fattah Capstone Report, Available at
https://github.com/datadiversitylab/city-3D-shapes/tree/main/docs/Capstone_report_for_H_M_Abdul_Fattah.pdf 
[9] Urban Heat Island dataset, 
Various UHI datasets available at
https://developers.google.com/earth-engine/datasets/tags/uhi  or 
Direct dataset download -
https://sedac.ciesin.columbia.edu/data/set/sdei-yceo-sfc-uhi-v4/data-download
Citation-
Center for International Earth Science Information Network - CIESIN - Columbia University. 2018. Gridded Population of the World, Version 4.11 (GPWv4): Population Count, Revision 11. Palisades, NY: NASA Socioeconomic Data and Applications Center (SEDAC). https://doi.org/10.7927/H4JW8BX5. Accessed 10/15/2024
[10] NOAA CDR AVHRR NDVI: Normalized Difference Vegetation Index, Version 5  dataset, available at
MODIS Combined 16-Day NDVI  available at
https://developers.google.com/earth-engine/datasets/catalog/MODIS_MCD43A4_006_NDVI 
[11] MCD18A1.061 Surface Radiation Daily/3-Hour dataset, Available at
https://developers.google.com/earth-engine/datasets/catalog/MODIS_061_MCD18A1  
[12] JRC Global Surface Water Mapping Layers, v1.4  dataset. Available at
https://developers.google.com/earth-engine/datasets/catalog/JRC_GSW1_4_YearlyHistory
Citation- 'Source: EC JRC/Google'
[13] GHSL - Global Human Settlement  Layer.  Available at
https://human-settlement.emergency.copernicus.eu/datasets.php 
(GHS-BUILT-H - R2023A dataset used for building height calculation)
[14] Kelso, N.V. and Patterson, T. (2012). World Urban Areas, LandScan, 1:10 million (2012). Available at
https://geo.nyu.edu/catalog/stanford-yk247bg4748 
[15] Elsen, PR., & Tingley, MW. (2015). Global mountain topography and the fate of montane 296 
species under climate change. Nature Climate Change, 5(8), 772-776 Available at
https://www.nature.com/articles/nclimate2656 
[16] One-Way ANOVA Test in R - Easy Guides - Wiki - STHDA Available at
https://www.sthda.com/english/wiki/one-way-anova-test-in-r 
[17] Kruskal-Wallis Test in R - Easy Guides - Wiki - STHDA  Available at
https://www.sthda.com/english/wiki/kruskal-wallis-test-in-r 
[18] Correlation matrix with ggally – the R Graph Gallery    Available at
https://r-graph-gallery.com/199-correlation-matrix-with-ggally.html 
 

### Acknowledgment

Initial project structure was created following the structure in [this repo](https://github.com/malill/research-template).
