---
layout: page
title: Details about UVAFME
---

## Scale and Spatial Interaction

Currently, UVAFME sites do not interact with one another and thus may be run in parallel or in sequence. Within a site, several hundred (generally 200) independent plots about the area of influence of a dominant tree crown (e.g. 500 m<sup>2</sup>) are simulated that represent patches of a forested landscape. Forest "landscape" in this context is defined as a dynamic mosaic of forest gaps (i.e. patches/plots) (see [Shugart et al. 1985](https://www.researchgate.net/publication/282756658_Modeling_Forest_Landscapes_and_the_Role_of_Disturbance_in_Ecosystems_and_Communities)). Within each patch, gap dynamics play out through the establishment of new trees following some major disturbance, growth and competition between trees to fill in the gap,  eventual dominance or co-dominance of a few trees, and death of such canopy dominants, which starts the cycle anew. Within UVAFME, the plots do not interact with one another, and thus represent independent replicates of potential forest dynamics occurring at a location with input environmental and climatological conditions. Due to the stochastic factors within UVAFME (i.e. disturbances, mortality, and regeneration), each plot will contain a forest patch undergoing some gap dynamics process, driven by both deterministic processes (e.g. tree growth response to external factors) and stochastic factors. A Monte Carlo-style average of such plots thus represents average, non-spatially explicit, per area *expected* forested conditions for the site location. This aggregation also produces emergent properties at the landscape scale (i.e. the average of several hundred gaps) such as forest succession, cyclical effects, and response to shifting climate and disturbance regimes.

![Scales](img/Scales_full.png)

Climate and daily weather conditions in UVAFME are the same across all plots within a site, thus each plot experiences the same temperature, precipitation, cloud cover, and PET each simulation day. As of Version 3 of UVAFME, soil conditions within each plot are independent of one another, driven by the plot-wide factors such as climate and input/initial soil conditions, as well as plot-specific factors such as forest cover and disturbances. Additionally, within each plot individual trees are placed on a 30x30 grid, but only interact spatially with one another with respect to insect infestation. Each plot is assumed to be horizontally (but not vertically) homogenous with respect to canopy cover and leaf area, seed rain and seedling banks, as well as soil conditions.

## Climate

Climate in UVAFME is simulated through input distributions of monthly temperature (ºC), precipitation (cm), and cloud cover (tenths of sky covered). The average monthly minimum and maximum temperatures, precipitation, and cloud cover, as well as standard deviations for these values (generally derived from at least 30 years of historical climate data) are used to create a range of possible values for a site in question. Monthly and daily weather conditions are the same across all plots within a site.
