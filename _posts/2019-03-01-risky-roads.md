---
title: Risky Roads Archive
subtitle: Presenting the results of a statewide motorist survey of dangerous intersections.
layout: default
modal-id: 3
date: 2019-03-01
img: risky-roads.png
thumbnail: thumbs/risky-roads-thumb.png
alt: 
project-date: March 2019
tech: VueJS, Mapbox-GL-JS, vector tiles
category: Freelance
description: 
---
This is a static website to present the results of a survey in which motorists were asked to identify dangerous roads across WA. The user can filter "spots" by council, electorate, suburb and so on. They can also download all the points within a given boundary as a CSV file.

To simplify long-term hosting, I built it without any server component. It is a simple static HTML/JavaScript site, with vector tiles hosted on Maptiler.com. To achieve the boundary filtering, I pre-processed the data, using vector tiles to calculate the boundaries for each point. I also pre-generated all the CSV files that could be downloaded, rather than computing them on the fly.

Live website: http://riskyroadsarchive.crowdspot.com.au/