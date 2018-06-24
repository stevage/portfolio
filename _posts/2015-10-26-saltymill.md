---
title: SaltyMill
subtitle: Automated deployment of full OpenStreetMap, PostGIS, TileMill, OSRM stack.
layout: default
modal-id: 3
date: 2015-10-26
img: saltymillp.ng
thumbnail: thumbs/saltymill-thumb.png
alt: 
project-date: 2014-15
tech: OpenStack, Salt, PostGIS, OSRM, Leaflet
category: Work and side project.
description: 
---
SaltyMill is a fairly complex SaltStack recipe that deploys a number of map-related components that can be very fiddly to set up and integrate manually. The complete stack it sets up:

- Can automatically download an OpenStreetMap extract for a given area.
- Loads that into PostGIS.
- Also fetches other data, such as OSM coastlines, and DEM terrain data.
- Provides TileMill, allowing users to create styled tile maps from all that data.
- Uses the Open Source Routing Machine to provide a routing service on that data.
- Provides an OSRM-Web front end, so people on the web can plan a route, using the customised tiles and data.

I built SaltyMill to solve two problems: 

1. managing the complex cycletour.org stack (and wanting to be able to rebuild it if necessary)
2. creating TileMill servers on demand for mapping workshops I was teaching under the researchmaps.net program.

A nice side-effect was that it was very easy to set up custom cycletour.org spin-offs for different areas overseas: Iceland, Scotland and Norway.

It worked fairly well, although I never felt that I got that much value out of using SaltStack. Using a series of Bash scripts and my own custom logic in Python or NodeJS would probably have been simpler, and required less time simply dealing with the specifics of Salt.

https://github.com/stevage/saltymill