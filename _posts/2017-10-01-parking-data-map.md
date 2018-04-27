---
title: Melbourne Parking Data Map
subtitle: Real-time visualisation of on-street parking space availability and restrictions.
layout: default
modal-id: 3
date: 2017-10-01
img: parking-map.png
thumbnail: thumbs/parking-map-thumb.png
alt: 
project-date: October 2017
tech: Mapbox-GL-JS, SQL
category: Salaried work
description: 
---
City of Melbourne's real-time parking data was released for the first time as open data in last 2017, the first local government (not counting ACT) to do so. To help potential users of the data make sense of it, I built an embeddable interactive map which visualises where the on-street spaces are, their current status (occupied or not), and their time restrictions. I also prepared some of the SQL queries, which are pretty complex.

Parking data is more complicated than you think: first, the relationship between physical infrastructure such as bays, spaces, signs, ticket machines, sensors. Next, restrictions are expressed for a variable number of time blocks covering different sections of each day, on different sets of days of the week - up to 6 different non-overlapping restrictions. Those restrictions include complications like loading zones, different time lengths for people with disabled permits, clearways, and so forth. And finally, there is the actual current status: occupied, non-occupied - and a couple of other statuses, such as out of use, and sensor apparently offline.

It's also challenging to convey two independent variables (status and restriction) for each point. We chose to use the interior of each circle to convey status, while the outer halo conveys the relevant restriction. Switching on the "disabled permit" checkbox alters the colour scheme. For instance, "disabled only" spots go from being grey to bright magenta, as now they are desirable.

See it here: [On-street parking data](http://www.melbourne.vic.gov.au/about-council/governance-transparency/open-data/Pages/on-street-parking-data.aspx).

[Source code on Github](https://github.com/City-of-Melbourne/parking-map/tree/gh-pages)