---
title: Smartygrants Maps
subtitle: Analyse and visualise grant data by boundaries such as LGA or Remoteness Area.
layout: default
modal-id: 3
date: 2018-09-01
img: oc-dashboard.gif
thumbnail: thumbs/oc-dashboard-thumb2.png
alt: 
project-date: 2018-09-01
tech: Mapbox-GL-JS, Java, Tippecanoe, GDAL
category: Paid employmnet
description: 
---
**SmartyGrants Maps** is an optional feature on the SmartyGrants platform which allows grantmakers to analyse their data by location, to answer questions like "are grantseekers overrepresented in certain local government areas" or "how does the remoteness of a grantseeker affect their chances of success?"

Adding a feature like this to a large existing codebase was complex, and required working with the team of Java developers. The major tasks involved:

* Scripts to download, clean, and process boundaries of many types into vector tiles.
* Also storing those boundaries within the main database, and developing routines to automatically geocode application locations against them.
* Extending the API to provide boundary location for applications to the dashboard.
* Building the dashboard itself, using Mapbox-GL-JS and the existing tech stack.

### Links

* [SmartyGrants Maps](https://www.smartygrants.com.au/sg/maps/) (marketing page with video)
