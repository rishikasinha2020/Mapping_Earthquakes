# Purpose
Basil and Sadhana like how you created your earthquake map with two different maps and the earthquake overlay. Now, Basil and Sadhana would like to see the earthquake data in relation to the tectonic plates’ location on the earth, and they would like to see all the earthquakes with a magnitude greater than 4.5 on the map, and they would like to see the data on a third map.

What We're Creating
This new assignment consists of three technical analysis deliverables. You will submit the following:

Deliverable 1: Add Tectonic Plate Data
Deliverable 2: Add Major Earthquake Data
Deliverable 3: Add an Additional Map

# Files/Data Set
Use the following links to download the Challenge starter code.

  Tectonic plate starter code.
  Major earthquake chart starter code.

# Deliverable 1: Add Tectonic Plate Data

Deliverable 1 Instructions
Using your knowledge of JavaScript, Leaflet.js, and geoJSON data, you’ll add tectonic plate data using d3.json(), add the data using the geoJSON() layer, set the tectonic plate LineString data to stand out on the map, and add the tectonic plate data to the overlay object with the earthquake data.

Create a new folder on your Mapping_Earthquakes repository and name it "Earthquake_Challenge."

Copy the folders and files from your Earthquakes_past7days branch and add them to the Earthquake_Challenge folder. The folder should have this structure:

    Earthquake_Challenge folder
      index.html
    static
      css
      style.css
    js
      config.js
      logic.js

In Step 1, add a second layer group variable for the tectonic plate data.

In Step 2, add a reference to the tectonic plate data to the overlay object.

In Step 3, using d3.json() callback method, make a call to the tectonic plate data using the GeoJSON/PB2002_boundaries.json data from this GitHub repository (Links to an external site.) for the tectonic plate data. You’ll need to log into GitHub to access the GeoJSON data.

Inside the d3.json() method do the following:

    Pass the tectonic plate data to the geoJSON() layer.
    Style the lines with a color and weight that will make it stand out on all maps.
    Add the tectonic layer group variable you created in Step 1 to the map, i.e., .addTo(tectonicPlates) and close the geoJSON() layer.
    Next, add the tectonic layer group variable to the map, i.e, tectonicPlates.addTo(map).
    Finally, close the d3.json() callback.
    Start your Python server and launch the index.html file and confirm that your map with the earthquake and tectonic plate data is similar to the following image.

Your final map should look similar to the following image:

All earthquake data  and  tectonic plate data on the map

Deliverable 1 Requirements
You will earn a perfect score for Deliverable 1 by completing all requirements below:

    The tectonic plate data is added as a second layer group

    The tectonic plate data is added to the overlay object
    The d3.json() callback is working and does the following:
    The tectonic plate data is passed to the geoJSON() layer
    The geoJSON() layer adds color and width to the tectonic plate lines
    The tectonic layer group variable is added to the map
    The earthquake data and tectonic plate data displayed on the map when the page loads

    # Refer to code: Mapping_Earthquakes\Earthquake_Challenge\static\js\challenge_logic.js
    # Refer to image: Mapping_Earthquakes\Resources\Image13.1.PNG


# Deliverable 2: Add Major Earthquake Data
Deliverable 2 Instructions
Using your knowledge of JavaScript, Leaflet.js, and geoJSON data, you’ll add major earthquake data to the map using d3.json(). You'll also add color and set the radius of the circle markers based on the magnitude of earthquake, and add a popup marker for each earthquake that displays the magnitude and location of the earthquake using the GeoJSON layer, geoJSON().


In Step 1, add a third layer group variable for the major earthquake data.
In Step 2, add a reference to the major earthquake data to the overlay object.
In Step 3, use the d3.json() callback method to make a call to the major earthquake data from the GeoJSON Summary Feed for M4.5+ Earthquakes (Links to an external site.) for the Past 7 Days.
In Step 4, use the same parameters in the styleInfo() function that will make a call to the getColor() and getRadius() functions.
In Step 5, change the getColor() function to use only three colors for the following magnitudes; magnitude less than 5, a magnitude greater than 5, and a magnitude greater than 6.
In Step 6, use the same parameters from the preceding step in the getRadius() function.
In Step 7, pass the major earthquake data into the GeoJSON layer and do the following with the geoJSON() layer:
Turn each feature into a circleMarker on the map
Style each circle with styleInfo() function

Create a popup for the circle to display the magnitude and location of the earthquake
Add the major earthquake layer group variable you created in Step 1 to the map, i.e., .addTo(majorEQ) and then close the geoJSON() layer.
Then, add the major earthquake layer group variable to the map, i.e, majorEQ.addTo(map), and then close the d3.json() callback.
Start your Python server and launch the index.html file and confirm that your map with the two earthquake data sets and tectonic plate data is similar to the following image.
All earthquakes, major earthquakes, and tectonic plate data on the map

# Deliverable 2 Requirements
You will earn a perfect score for Deliverable 2 by completing all requirements below:

The major earthquake data is added as a third layer group
The major earthquake data is added to the overlay object
The d3.json() callback is working and does the following:

    Sets the color and diameter of each earthquake.
    The major earthquake data is passed to the geoJSON() layer.
    The geoJSON() layer creates a circle for each major earthquake, and adds a popup for each circle to display the magnitude and location of the earthquake
    The major earthquake layer group variable is added to the map
    All the earthquake data and tectonic plate data are displayed on the map when the page loads and the datasets can be toggled on or off
 
 # Refer to code: Mapping_Earthquakes\Earthquake_Challenge\static\js\challenge_logic.js
 # Refer to image: Mapping_Earthquakes\Resources\Image13.1.PNG

# Deliverable 3: Add an Additional Map
Deliverable 3 Instructions
Using your knowledge of JavaScript and Leaflet.js add a third map style to your earthquake map.

Deliverable 3 Requirements
You will earn a perfect score for Deliverable 3 by completing all requirements below:

A third map tile layer is created
The third map is added to the overlay object
All the earthquake data and tectonic plate data are displayed on the all maps of the webpage

 # Refer to code: Mapping_Earthquakes\Earthquake_Challenge\static\js\challenge_logic.js
 # Refer to image: Mapping_Earthquakes\Resources\Image13.2.PNG