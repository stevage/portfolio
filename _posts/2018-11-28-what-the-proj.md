---
title: What the Proj?
subtitle: Helps guess the correct projection given an easting-northing pair and an approximate lat-lon.
layout: default
modal-id: 3
date: 2018-11-28
img: what-the-proj.png
thumbnail: thumbs/what-the-proj-thumb.png
alt: 
project-date: November 2018
tech: VueJS, proj4
category: Hobby project
description: 
---
Sometimes you come across some geospatial data that is in an unknown projection. There is no readily available tool which helps solve this problem.

This quick website provides one solution. You enter the (X, Y) coordinates of one of your points, and the (lon, lat) of your best guess as to where the point should project be. (Presumably you know *something* about the location of the data!) *What the Proj* then tries every projection it knows to see which is closest.

## Links: 

* [Source code on Github](https://github.com/stevage/whattheproj)
* Play with it in online: https://stevage.github.io/WhatTheProj/
