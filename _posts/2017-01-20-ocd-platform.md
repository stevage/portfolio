---
title: Open Council Data Aggregator
subtitle: Platform that automatically finds, acquires, merges, publishes open data from dozens of local governments.
layout: default
modal-id: 3
date: 2017-01-20
img: ocd-platform.png
thumbnail: thumbs/ocd-platform-thumb.png
alt: 
project-date: 2017-01-20
tech: NodeJS, Material Design Lite, Cloudant (CouchDB), Mapbox-GL-jS
category: Paid employment.
description: 
---
The Open Council Data Aggregator was a prototype platform that solves the problem of scale for local government data. Using the growing number of open datasets published by local governments that follow the [Open Council Data Standards](https://standards.opencouncildata.org), it produces a simple endpoint where a given dataset (such as garbage collection zones) can be queried, without concern for where each council originally published that dataset.

The idea was originally workshopped through an REA (realestate.com.au) internal hackathon, then I redeveloped it from scratch while working at the City of Melbourne. How it works:

- Each "topic" (such as Public Toilets) is defined by a tiny set of parameters, such as its name and keywords to search for.
- The aggregator searches a number of known locations for council open data presences, looking for these topics.
- All the matching datasets are downloaded, converted to GeoJSON, and aggregated into a single topic GeoJSON.
- That file is uploaded to Mapbox for display, and also to IBM Cloudant for querying.
- Other Cloudant queries allow asnwering questions like "How many councils support this topic".
- A front end, built using Google's "Material Design Lite", lets developers see the current state of each topic, and lets data publishers see whether their data meets the standard.

### Links

* Back end (Github): https://github.com/OpenCouncilData/Aggregator
* Front end (Github): https://github.com/opencouncildata/Platform
* Live site: https://opencouncildata.github.io/Platform/ (Partially non-functional due to Cloudant retiring their free plan)
