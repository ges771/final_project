# Project Overview
My GES class project is a webmap that shows the locations of a housing program's funded properties. I represent the properties by the type of project their funding assisted. Users can export additional data about the projects as a csv and export the map view as an image.

# Description
The original spreadsheet was processed in python using the code in the clean_data.py file. I removed uneccesary fields and changed that data types to make them internally consistent. Using the masked X and Y fields to create points, the spreadsheet was cleaned and converted into a geodataframe and exported to a CMF2019data geoJSON and csv file. The geoJSON was the uploaded to mapbox to use as a tileset.

The project uses Mapbox GL JS to display the project addresses,  and uses Mapbox's basic style as a background static layer. I based my code on the exampels found here: https://docs.mapbox.com/mapbox-gl-js/examples/#user-interaction. The data and background were referenced using a key-token pair from Mapbox
