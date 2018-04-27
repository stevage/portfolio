---
title: SchoolScape
subtitle: Visualisation tool for school planners, combining demographic change and school infrastructure.
layout: default
modal-id: 3
date: 2018-02-25
img: schoolscape.png
thumbnail: thumbs/schoolscape-thumb2.png
alt: 
project-date: February 2018
tech: Mapbox-GL-JS, Vector tiles (Tippecanoe), VueJS, NodeJS
category: Contract
description: 
---
This project, ultimately for the Victoria Department of Education, helps school planners allocate resources, by visualising the best 
available information.  That includes where school-aged children live, the proportion of them that attend government schools, 
the existing school infrastructure, and how much (if any) spare capacity there is.

The data is made more complex by the number of dimensions along which data can be analysed:
- Year (2018 to 2037)
- Year level (Prep to Year 12)
- Two different scenarios which contain different assumptions for future projections.
- Many different geographic boundary types, such as Statistical Areas (1,2,3,4), Local Government Areas, Suburbs, and department-specific reporting areas.

I built the front end using VueJS and Mapbox-GL-JS. It's essentially a static site, using pre-baked vector tiles jam-packed with as many data attributes as possible. A fully automated pipeline of NodeJS scripts uses Tippecanoe to generate these vector tiles, combining data provided as Shapefiles and CSV.
