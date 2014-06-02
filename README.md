![PATH trains](/Screenshots/PATH-lines.png?raw=true "PATH trains")

An open map of mass transit for Hudson County, NJ. 

Created for [Open Jersey City](http://openjerseycity.org/ "Open Jersey City") as part of the [Hack for Change National Day of Civic Hacking](http://openjerseycity.org/Transportation-Hackathon-2014/ "Hack for Change National Day of Civic Hacking"). 

Built in QGIS. http://qgis.org/

#About the project:
Hudson County residents are some of the most frequent users of public transportation nationwide, but there's currently no single source for detailed transit information in the area: data is split between individual carriers, each with their own format and method of access, and service outages can leave riders with no easy way to find alternate routes home. The lack of easily accessible transit information is particularly a problem for the communities served by smaller operators. Word of mouth is a more reliable source of schedules and stops than any of their websites -- one carrier's page consists of a single PDF of a scanned printout of a timetable.

The goal of this project is to create a central mapping repository covering all transit services within Hudson County. While usable for transit navigation in its current form, this map is really designed to lay the groundwork for bigger projects. The datasets have been organized into layers by mode of conveyance. With all of them enabled it's a little bit overwhelming:

![Everything At Once](/Screenshots/all-layers-enabled.png?raw=true "Everything At Once")

Much of the day was devoted to extracting Hudson-only data from NJ Transit's massive statewide bus dataset, which initially contained over three million shape points!


##Data added so far:
- PATH lines and stations
- Hudson-Bergen Light Rail lines and stations
- NJ Transit Bus lines and bus stops
- NY Waterway Ferry routes
- NJ Transit Rail lines and stations
- Jitney (Dollar Van) Bus Routes (compiled by another OpenJC hackathon team as part of their awesome project: https://github.com/OpenJC/Jitney)
- Newark City Subway/Light Rail lines
- AirTrain EWR
- Base map layer (via OpenStreetMap and NationalAtlas.gov)
- Accessibility info for PATH and HBLR stations


##Hoping to add:
- Hoboken HOP bus
- Red & Tan buses (Operated by CoachUSA, have yet to find any route data newer than 2010)
- Ferry terminals
- Liberty Landing Ferry
- NJT Bus Route lines connected to bus numbers (and possibly their destinations outside Hudson County)
- Meadowlands Rail Line (NJT)
- Bike lanes
- Connections to NYC Subway
- Schedules and realtime data

##Future plans:
- Improve design and data hierarchy to make the information easier to navigate
- Use this map to generate a layered set of map tiles for interactive web use

##More Screenshots:
![Base Map](/Screenshots/base-map_with-ferries.png?raw=true "Base Map")
Base Map

![Jitney Bus Routes](/Screenshots/jitney-routes.png?raw=true "Jitney Bus Routes")
Jitney Bus Routes

![NJ Transit Buses](/Screenshots/NJT_buses-and-stops.png?raw=true "NJ Transit Buses")
NJ Transit Buses

![Hudson-Bergen Light Rail](/Screenshots/HBLR.png?raw=true "Hudson-Bergen Light Rail")
Hudson-Bergen Light Rail

![Connections to EWR Airtrain](/Screenshots/connections-to-airtrain.png?raw=true "Connections to EWR Airtrain")
Connections to EWR Airtrain

![All Currently Available Layers](/Screenshots/layers.png?raw=true "All Currently Available Layers")
All Currently Available Layers