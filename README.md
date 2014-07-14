﻿#Hudson County Open Transit Map

![Hudson County Open Transit Map](/Screenshots/new-new-header-image.png?raw=true "Hudson County Open Transit Map")

An open map of mass transit for Hudson County, NJ. 

Created for [Open Jersey City](http://openjerseycity.org/ "Open Jersey City") as part of the [Hack for Change National Day of Civic Hacking](http://openjerseycity.org/Transportation-Hackathon-2014/ "Hack for Change National Day of Civic Hacking"). 

Built in QGIS. http://qgis.org/

#About the project:
Hudson County residents are some of the most frequent users of public transportation nationwide, but there's currently no single source for detailed transit information in the area: data is split between individual carriers, each with their own format and method of access, and service outages can leave riders with no easy way to find alternate routes home. The lack of easily accessible transit information is particularly a problem for the communities served by smaller operators. Word of mouth is a more reliable source of schedules and stops than some of their websites -- one carrier's page consists of a single PDF of a scanned printout of a timetable.

The goal of this project is to create a central GIS repository covering all public transportation services within Hudson County. While usable for transit navigation in its current form, this map is really designed to lay the groundwork for bigger projects. Everything is vector-based, much of the data is tagged with attributes, and the datasets have been organized into layers by mode of conveyance. With all of them enabled at once it can get a little bit overwhelming:

![Everything At Once](/Screenshots/all-layers-enabled-v2.png?raw=true "Everything At Once")

That data, however, can be selectively enabled and filtered to produce much more useful maps. These can range from basic guides for visitors, such as this simple PATH service map...

![Weekday PATH service](/Screenshots/path-weekdays.png?raw=true "Weekday PATH service")

...to visualizations that could affect policy, such as this one that reveals a large section of Jersey City that lacks direct access to NYC via bus. 

![No buses to Midtown](/Screenshots/no-buses-to-pabt.png?raw=true "No buses to Midtown :-(")

After Hurricane Sandy disrupted train service for several weeks, residents of this neighborhood faced particularly serious issues getting to work.

All resulting shapefiles are standard WGS84 projections. Many include connections and key destinations beyond Hudson County, such as Newark Airport. Individual layer style files are also included.

The hack day was largely devoted to processing and simplifying very large sets of data, including extracting Hudson-only data from NJ Transit's massive statewide bus dataset, which initially contained over three million shapes! Much of the data has since been further cleaned, sorted and reformatted.


##Data added so far:
####Rail
- PATH lines and stations, including weekend service
- Hudson-Bergen Light Rail lines and stations
- NJ Transit Rail lines and stations
- Newark City Subway/Light Rail lines
- AirTrain EWR (via OpenStreetMap)
- Accessibility info for PATH and HBLR stations

####Buses
- NJ Transit Bus lines and bus stops
- [A&C Buses](http://acbuscorp.com/index.html)
- [Decamp Bus Lines](https://maps.google.com/maps/user?uid=215431211415581436371&hl=en&gl=us&ptab=2)
- Jitney (Dollar Van) Bus Routes (compiled by another OpenJC hackathon team as part of their awesome project: https://github.com/OpenJC/Jitney)

####Ferries
- NY Waterway Ferry routes and terminals (Newport removed)
- Liberty Landing Ferry
- Statue Cruises (Ferries to Ellis Island and the Statue of Liberty)

####Base Map Layers
- Two base map layers, one simple and one highly detailed (via OpenStreetMap, NJGIN and NationalAtlas.gov). Detailed map includes municipal borders, streets, parks, water features, pedestrian footpaths, major buildings, harbor islands and surrounding counties.

*All data sourced from transit operators and OpenStreetMap unless otherwise indicated.*


##Hoping to add:
- Hoboken HOP bus
- NY Waterway buses
- [State Transtours'](http://statetranstours.com/) [Society Hill Shuttle](http://society-hill.com/transportation.html) 
- [Trans-Bridge Lines to PA](http://www.transbridgelines.com/daily.htm)
- Red & Tan buses (Operated by CoachUSA, have yet to find any route data newer than 2010, may no longer be running in Hudson County). Broadway IBOA is another possible single-route carrier?
- Bike lanes (may need to crowdsource info on new lanes in Jersey City)
- Higher-resolution jitney routes
- Additional connections to NYC Subway
- Schedules and realtime data

##Future plans:
- Improve design, layout and data hierarchy to make the information easier to navigate at different scales and levels of detail
- Add more (and more detailed) metadata to the layer attribute tables
- Link GTFS shapes to route information
- Use this map to generate a layered set of map tiles for interactive web access

#More Screenshots:
![Base Map](/Screenshots/base-map_with-ferries-v2.png?raw=true "Base Map")
Base Map

![Downtown Jersey City](/Screenshots/downtown-JC.png?raw=true "PATH trains")
Downtown Jersey City

![Harrison and Newark](/Screenshots/harrison.png?raw=true "Harrison and Newark")
Harrison and Newark

![Hoboken Terminal](/Screenshots/hoboken-trains.png?raw=true "Hoboken Terminal")
Hoboken Terminal

##Older Screenshots:
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