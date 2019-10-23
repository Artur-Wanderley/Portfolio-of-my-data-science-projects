# Data preparation to model plant species distribution in the Brazilian Caatinga dry forest in response to climate change and other human disturbances¶
This project is part of an academic research in which I am collaborating. The research involves [Dr. Bruno Pinho](https://www.researchgate.net/profile/Bruno_Pinho3), [Professor Marcelo Tabarelli](https://www.researchgate.net/profile/Marcelo_Tabarelli) (both from the Federal University of Pernambuco - Brazil) and [Professor Carlos Peres](https://www.researchgate.net/profile/Carlos_Peres), from the University of East Anglia - United Kingdom.

The goal of this academic research is to understand the extent to which plant species from the Brazilian Caatinga dry forest are threatened by climate change and human activities. To reach this goal, we will build a predictive model to predict which flora (in terms of species number and composition) we can expect in the near future, given specific climate and human disturbance conditions.

In this project, we will perform some data manipulation to convert the raw data we have into a dataset appropriate to build a predictive model. 

Specifically we will:.

- Write the to_bin function to create 50 km2 bins (the grid cells)
- Use map(to_bin) on the geographic coordinates to create the 50 km2 grid cells
- Calculate the geographic coordinates of the center of each grid cell (centroids)
- Use pandas.DataFrame.groupby to group the species occurrences into the grid cells
- Use pandas.DataFrame.pivot to convert our dataset into a species abundance matrix in which each column is a plant species and each row is a grid cell.
- Use pandas.DataFrame.merge to combine different datasets
- Do some data cleaning through string manipulation: string format() and regex
- Use for loop and zip() function to rename hundreds of column labels at once
- Use the Matplotlib Basemap Toolkit to plot our data into a geographic map


## Note:

We will make the dataset used in this project publically available upon the publication of the full research in a scientific journal.
