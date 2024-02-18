# Leaflet Challenge
This challenge revolves around visualizing interactive data from the USGS using the leaflet plugin with JavaScript and the D3 library. The goal is to map out earthquake data. The parameters I chose were earthquakes of magnitude 4.5+ in the last 30 days.

## Method
First, I set the API link as a constant variable in order to load the data into the functions I planned to create for each chart. I based almost all of this code on the basic and advanced CitiBike mini project we completed in class for lesson 3 of module 15. I followed the logic and structure and tweaked it to fit the requirements of this project. 

I used a ‘createMap’ function to add my tiles, base maps , overlay map, to access the plate boundary data, and to create the legend. I then created a function, ‘earthquakeMarkers’, to create and customize the earthquake markers by depth and magnitude, as well as add a popup upon clicking feature to show more details of that particular earthquake. I was having issues with the date and had to research how to convert the provided date into a format the everyday person understood as a date and came across the Date.ToUTCString() function which worked well. To finish up the earthquakeMarkers function, I connected the earthquake data from the JSON to the markers. 

Lastly, I created a function to insert the legend in the HTML using the querySelector() and innerHTML() functions. I also researched how to adjust the color of the text in the legend and found a resource that showed me how to do so in the CSS file. 

![earthquake_map](https://github.com/ASPigman/leaflet_challenge/assets/145923874/4c5870e0-d23a-40b9-8fe2-9fe3974beab7)


## Acknowledgements
Othmane Benyoucef - Instructor for Tulsa Community College Data Analytics Accelerated Training Program

Kaylie Butler - TA

Jacob Peroutek - TA

EdX Bootcamps

<a href="https://plnkr.co/edit/qAjh0duPRI4US6Q4DSCN?p=preview&preview" target="_blank">Adjusting font color for legend in CSS</a>
