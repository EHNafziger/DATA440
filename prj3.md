# Project 3 - Final
  
## London Gravity Model Analysis

To practice implementing a gravity model, I followed the exercise laid out in Adam Dennett's "Dr Ds Idiots Guide to Spatial Interaction Modelling for Dummies - Part 1: The Unconstrained (Total Constrained) Model." The area of focus is the city of London (England). Using json data availible from the United Kingdom's government statistics, I organized the borough's into coded regions. I then imported commuting, population, and income data from a provided dropbox link. The data was then organized by borough code.

![](cdata_head.png)

Due to package bugs, I did not run the travel network as an animation (the class was told not to) but a sample of the final data is below. Population and income data was used to determine movement in this gravity model output, essentially weighing the chances  of an individual moving from one region to another. The matrix illustrates the number of individuals that migrated from one borough to another as determined by the model's parameters of population and income.

![](london_matrix.png)

## ABM of Guatemala

Since I have used Guatemala as my area of focus this entire semester, I see no reason to change it up now. In the Garcia et al. paper we discussed in class, a similar model to what I will be displaying here was used to estimate population flow. The major difference is my model uses recorded migration data to inform flow. Using migration data from WorldPop.org, I created shapefiles of the flow of migration, both in terms of its origin and its destination. I then combined these two dataframes to illustrate simplified migration routes between all states in Guatemala. These originate at each states centerpoint.

![](origins.png)![](destinatinos.png)

![](od_lines.png)

After setting up these initial parameters, I distributed points across Guatemala roughly equivalent to the population distriubtion (shown below). The distribution of these points could be done differently; for example, using raster data to inform distribution would make this more accurate. The two animations are the same except I have removed the migration lines in one for more clarity.

![](gtm_and_bar.png)

![](abm.gif) ![](abm_nls.gif)

It would be useful in cases to where there is not traffic or migration data to have other predictors, possibly remotely gathered, which would be able to inform researchers of population migration in the region. Night lights are one example which can be gathered remotely and indicate a higher population density, as well as potentially a higher standard of living, which is a desirable pull factor.

## Voronoi Polygon of the Barberena and Cuilapa Municipalities

Below is the Voronoi polygon produced for the municipalities of Barberena nad Cuilapa in the State of Santa Rosa. To produce an origin/destination matrix like the one produced for London, I would just need to subset the WorldPop.org data used to generate the ABM of migration in the country of Guatemala. Data should be available at this level of government (adm2). The centerpoints are already defined as part of the Voronoi projection, and path/directionality could be determined in the same way as the Guatemala ABM above. Different weights aside from migration data could be incorporated, such as the already mentioned night lights or the presence of infrastructure such as roads and hospitals (as we definied in Project 1). Furthermore, transportation methods could be incorporated to draw migration and direct it, as this is what happens in the real world.

![](rosa_voronoi.png)
