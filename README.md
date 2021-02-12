# UsAirportsWebMap
Web Map Link: https://dhritiy.github.io/UsAirportsWebMap/

![Map of US Airports](https://github.com/dhritiy/UsAirportsWebMap/blob/main/img/US%20Airports%20Map.PNG)

For this project I created a map of airports across the United States, including Hawaii, Alaska, and outlying islands. I also wanted to display whether these airports had control towers or not, because the ones that do have them, use control towers to direct air traffic.

I used several different functions to create this web map. One of the most important ones was pointToLayer(). This function alters the default marker that comes with GeoJSON points. I passed in my feature(aiports) and coordinates to this layer and then wrote an if() statement to determine whether that airport has control tower. Then I assigned a new marker that would be in the shape of plane. This allowed me to customize the shape and color of the marker. I chose one color blue to mean the airport has a control tower, and purple to indicate that it does not. I also used the onEachFeature() function to attach a popup to each airplane marker. When you click on an airplane, you are able to see the name of the airport, but also the name of the city and state. This is to give the viewer more context to the location of the aiport. I also created a function in order to help determine the color scheme of the US-states based on number of airports in each state and also another one to determine the style.

The airport dataset was from the USGS and the data for US states was from Mike Bostock at Data-Driven Documents. I also used a basemap that was from OpenStreetMap. Some of the libraries that I used were Google Fonts, Chroma.js in order to color the map, and the JavaScript leaflet.ajax library. 
