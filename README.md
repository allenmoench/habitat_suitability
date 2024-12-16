# habitat_suitability

[![DOI](https://zenodo.org/badge/893246169.svg)](https://doi.org/10.5281/zenodo.14497285)

In this project I will analyze the effect of climactic changes on the habitat of Sorghastrum grass species. Changing climate may have caused changes to soil health, temperature, precipitation, or other factors that may be changing the traditional range of species distribution for Sorghastrum. I will create a reproducible workflow to analyze whether this is the case, and to provide a template that can be used to aks the same question for different species.

To run the code, begin with the first notebook (01_grassland_selection). If the study area is one of the grasslands from "grasslands_gdf", then the code should be able to be run as-is, only changing the NATIONALGR value in the code cells that define and plot the grassland boundaries. If study areas outside the grasslands_gdf are being used, additional changes will be required.

In the second notebook (02), it should be possible to simply "run all", although for a new study area the latitude and longitude values would need to be changed. In future runs using different study areas, the object names may become misleading since they refer to Pawnee and Comanche grasslands. Changing these names might help to maintain consistency, however I recommend against it since the names Pawnee and Comanche (sometimes denoted by p or c in the object name) are also used in future notebooks which means that those would need to be changed as well for the code to continue to function.

Notebook 02a should be possible to run simply via "run all".

In notebook 03, the pattern used to identify DEM tiles will likely need to be modified for future runs on different study areas, since Lat and Long values are coded into the data in some cases.

For future runs of notebook 04, it should be possible to change the variables indicated to new values, by deleting the current values and typing in the new ones (for example, replace pr with pH or change start year from 2096 to 2091). 

Notebook 05 contains an incomplete fuzzy logic model code. It's intended to create a suitability score raster composed of numbers between 1 and 0. This is different from the suitability score raster in notebook 06, in that it presents a range of decimals instead of an array of integer ones and zeroes. This notebook is incomplete, and likely won't run properly. For future studies, it may be possible to edit this and run it so that it completes correctly.

Notebook 06 should be possible to run using "run all", although variables such as start_year, end_year, and others will need to be updated as new values are tested. Also, tolerance values and optimal growing conditions for the species in question will need to be updated. 