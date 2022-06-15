# Boston_MBTA

My final project looks at the Metro Boston Transit Authority (MBTA) and state-designated Environmental Justice communities in Massachusetts.

One of the benefits of using data sourced from MassGIS (Bureau of Geographic Information), is that almost all of their data and layers are available to view in an onine map. That way, I could preview the data and get a feel for what information was going to be most helpful for the project I am interested in.

I first navigated to the MassGIS website to check out what data is availabe for download. You can find all the files here: https://www.mass.gov/info-details/massgis-data-layers

There are a number of zip files I dowloaded from these pages to start my map. In bottom to top order-
1: Municipalities (Political/Administrative Boundaries)
2: 2020 Environmental Justice Populations (Census Data)
3: Protected and Recreational Open Space (Conservation/Recreation)
4: MBTA Rapid Transit (Infrastructure)

Many of these zip files have multiple shapefiles in them, several of which may be useful. for my projects, I used townssurvey_shp — TOWNSSURVEY_POLYM_GENCOAST.shp, ej2020 — EJ_2020_POLY.shp, openspace — OPENSPACE_POLY.shp, and mbta_rapid_transit — MBTA_NODE.shp. It's helpful to rename these layers now so they can be distinguished from the others. I don't aways like to remove extra layers in case they may be helpful later on.

After I've renamed the layers I'm using, I went on and styled them to make them easier to read. I changed the project background to a blue water color, and the municipalities layer to a dark green with light grey boundaries. I changed the EJ Neighborhoods to a light cream color and opacity and color of the parks to a lighter green and removed the boundaries so they could be seen across the neighborhoods on the EJ layer. Last, I changed the colors of the MBTA Stations to the colors associated with their train lines. all the official hex code colors can be found here: https://en.wikipedia.org/wiki/Module:Adjacent_stations/MBTA/sandbox

I have also saved a new style in my repo for colorizing the different train stops according to official MBTA colors.

For this project I want to mainly focus on the rapid transit trains rather than buses because the bus system provides a significantly less reliable service and is dependent a far more factors (traffic, weather, road construction, etc.) than the trains. If my map is about effective accessibility, expanding train services would have a much greater impact on underserved communities than additional bus stops and routes, (in my opinion). 

Now that the map layers are in order and styled, I want to take a look at areas that are within .5 miles of any train stations, which would be about a 10-minute walk. I started with using buffers to identify what that radius looks like.



