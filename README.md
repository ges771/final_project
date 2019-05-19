# Project Overview
My GES class project is a webmap that shows the locations of a housing program's funded properties. I represent the properties by the type of project their funding assisted. Users can export additional data about the projects as a csv and export the map view as an image.

# Description
This project is based on a task I did for work, with more limited functionality and in a less complete form. Some parts are intentionally vague for that reason.

The original spreadsheet was processed in python using the code in the clean_data.py file. I removed uneccesary fields and changed that data types to make them internally consistent. Using the masked X and Y fields to create points, the spreadsheet was cleaned and converted into a geodataframe and exported to a CMF2019data geoJSON and CSV file. The geoJSON was the uploaded to mapbox to use as a tileset.

The project uses Mapbox GL JS to display the project addresses,  and uses Mapbox's basic style as a background static layer. I based my code on the exampels found here: https://docs.mapbox.com/mapbox-gl-js/examples/#user-interaction. I referenced the data and background using a key-token pair from Mapbox, and styled the data and legend following the style tutotrials. I used the 'Project Type' column to create catagories to be displayed. 

The buttons were created using functions referencing javascript libraries, and are styled after code provided to me for reference. The csv columns are exported manually, and the image is prited out using a library with as SaveAs function.

The Mapbox styling is done in Javascript nested within an HTML document. This HML file is names cmf_map.html, and serves as the master script for the webmap. You can see the final map here: https://docs.mapbox.com/mapbox-gl-js/examples/#user-interaction. 


