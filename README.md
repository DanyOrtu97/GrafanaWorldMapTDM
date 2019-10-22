# WorldMapTDM
Authors: Daniele Ortu, Gabriele Merlin, Gianmarco Cherchi and Riccardo Scateni (University of Cagliari, Italy)

This plugin is part of the TDM project (http://www.tdm-project.it) and it has been presented during the STAG 2019 scientific conference (http://stag2019.crs4.it) with the poster "Design and Implementation of a Visualization Tool for the in-depth Analysis of the Domestic Electricity Consumption".

###################
Previous version of WorldMap Panel
###################

Read more about it here:
https://grafana.com/grafana/plugins/grafana-worldmap-panel/installation



###################
Modified version of WorldMapPanel
###################

WorldMapTDM is a modified version of Grafana’s native worldmap panel. It is a part of TDM project, (link: http://www.tdm-project.it/), initiative born thanks to the collaboration between CRS4 and the University of Cagliari.
In this case, the goal was to show a map of Cagliari divided into zones, in this way is possible to select, using the map, an area of interest, to make comparisons between own consumption and those of the houses in the selected area.

###################
Limits of native panel
###################

The original worldmap did not allow division into zones and selection of a zone, but only allowed to create circles in the map through a query, representing a value for a given area. The query in question should provide geographical coordinates.

###################
What’s new
###################

This version of WorldMap Panel presents a map of Cagliari divided into zones, in which each zone can be selected. The only query present is now used for the association between houses and zones.
A mode selection button has also been added to allow the change of mode:
selection of the whole city
selection by zones

###################
Setup on Grafana(Windows)
###################

To use this plugin inside Grafana it is necessary to download it, unzip it and insert it into Grafana installation folder: grafana-5.4.2 -> data -> plugins 
To configure it on Grafana you need the support to a database as Influxdb or similar. After database configuration, the only query must be entered as in the old plugin, but in this modified plugin it is necessary to have a query that generates the association between houses and zones.



