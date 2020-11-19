# Project 3 - Final
  
## London Gravity Model Analysis

To practice implementing a gravity model, I followed the exercise laid out in Adam Dennett's "Dr Ds Idiots Guide to Spatial Interaction Modelling for Dummies - Part 1: The Unconstrained (Total Constrained) Model." The area of focus is the city of London (England). Using json data availible from the United Kingdom's government statistics, I organized the borough's into coded regions. I then imported commuting, population, and income data from a provided dropbox link. The data was then organized by borough code.

![](cdata_head.png)

Due to package bugs, I did not run the travel network as an animation (the class was told not to) but a sample of the final is below. Population and income data was used to determine movement in this gravity model output. The matrix illustrates the number of individuals that migrated from one borough to another as determined by the model's parameters of population and income.

![](london_matrix.png)

## ABM of Guatemala

![](origins.png)![](destinatoins.png)

![](od_lines.png)



![](abm.gif) ![](abm_nls.gif)
