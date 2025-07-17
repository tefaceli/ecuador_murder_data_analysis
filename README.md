# Murders in Ecuador

This repository includes the analysis of data on intentional homicides in Ecuador between 2023 and May 2025. The information used for the analysis was obtained from the [Ecuadorian Government’s Open Data Portal](https://datosabiertos.gob.ec/dataset/homicidios-intencionales).

"The goal of this project is to provide a deeper analysis of violent deaths in Ecuador. Typically, analyses are carried out at the provincial or cantonal level. However, this repository includes analysis at the parish and neighborhood levels.

To perform the geospatial analysis, I used shapefiles from the National Electoral Council (CNE), with two types of divisions:

- Parishes, which are official administrative units.
- Electoral zones, which are not official administrative divisions, but are used by the CNE for electoral processes. These zones serve as a proxy for defining neighborhoods in the most populated cities.

The shapefiles were obteined [here](https://github.com/pablovelascoec/espacial_elecciones_Ec). 

The analysis conducted in this project revealed several key findings:
1. Parishes in Guayaquil and Durán recorded the highest numbers of deaths.
2. The parish with the longest streak of daily homicides is Pascuales, in Guayaquil, with 22 consecutive days.
3. Pascuales also saw as many as 22 murders in a single day.
4. Divino Niño parish, in Durán, is one of the most violent despite its small size.

For this project, I used geopandas and shapely geometry for the geospatial analysis. T found that option better than using QGIS, since I could esaily do data analyisis in Python.

This was done in two Jupyter Notebooks:
1. The first one includes the cleaning and joining of two datasets, one for historical data and one for 2025.
2. The second one includes the geospatial analysis of the clean data.

This is a preliminary analysis of violence in Ecuador at a micro level, focusing on small areas where citizens are most affected. Future analyses should combine parish-level data with census information to calculate homicide rates for each parish.

This project was developed as part of the LEDE Program, at Columbia Journalism School.