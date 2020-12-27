# world-population-visualization

first import these (if not installed install all of them by 'pip install')
  import os
  import glob
  import dbfread
  import matplotlib.pyplot as plt
  import pandas as pd
  import geopandas as gpd
  
second, read the shapefile(specifically columns 'ADM0_A3'(country codes) & 'geometry' -> geod.read_file(shapefile)
  you can also check the column names by this command if column name not in index error occurs -> list(origdf.columns.values)
  
third, read the csv data file(specifically columns 'Country Code' & '2019'(population) -> pd.read_csv(datafile)

fourth, merge the two files on columns - 'ADM0_A3' & 'Country Code'

fifth, plot the map according to the population in color shading.
