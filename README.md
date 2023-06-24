# Akron Unbuildable Lots Project
See my website for in-depth discussion of the purpose and conclusions of the project [here](https://gracejulien.github.io/projects/akron_unbuildable).
## Data
Almost all of the data used for this project is included in zipped_data; to use this with the Jupyter notebook files, unzip all of the folders, and copy all of the data into a single folder titled 'data'. I had issues with github's file size limit, which is why this is somewhat unintuitive. The tax parcel data (Tax_parcels.dbf, etc.) was too large even when zipped. It can be downloaded [here](https://data-summitgis.opendata.arcgis.com/datasets/summitgis::parcels-web-geodata-tax-parcels/explore).
## Visuals
The static maps generated using QGIS (see map.qgz) are in the visuals folder. The dynamic maps generated using Python, GeoPandas, and Folium (see generate_visuals.ipynb) are in the interactive_visuals folder.
## Code
### generate_data.ipynb
Included in this is my process to create several datasets, including akron_juris (the City of Akron's jurisdiction boundaries), akron_roads (roads within the City of Akron), and, most importantly, akron_frontage_25to45 (all parcels in the City of Akron with frontage between 25 ft and 45 ft).
### generate_visuals.ipynb
Included in this is my process to create the dynamic maps included in interactive visuals. There are three maps created: front_all, which has all of the "unbuildable" parcels in the city color-coded by vacancy status, front_occupied, which has all of the "unbuildable" parcels in the city that have residential buildings, and front_vacant, which has all of the "unbuildable" parcels in the city that are vacant.
### map.gqz
This is a QGIS file. This is how I made the static maps included in the visuals folder.
