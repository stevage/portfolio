---
title: getlon.lat
subtitle: Recommends geocoder plans based on your specific needs
layout: default
modal-id: 3
date: 2018-04-01
img: ocd-which-geocoder.png
thumbnail: thumbs/ocd-which-geocoder-thumb.png
alt: 
project-date: 2018-04-01
tech: VueJS
category: Paid employment turned side project.
description: 
---
**getlon.lat** is a tool for choosing between the dozens of different geocoding APIs on the market, and their many different pricing plans. I developed it in the process of researching plans, while working at [Our Community](http://ourcommunity.com.au). Reading the fine print, there are many restrictions on geocoding services which aren't immediately obvious. These include:

* Not being able to store geocodes, either at all, or beyond 30 days.
* Not being able to display geocodes on map tiles from competitors.
* Not being able to display geocodes using any other service at all.
* Not being able to display the actual latitude and longitudes.
* Not being able to combine geocodes with other forms of data.
* Not being able to use the service in a commercial context.

And many others.

Technically, the site is not very complicated. The complication arises from developing a generic formula for calculating the expected monthly fee, given all the many different variables, in a way that is roughly fair to every provider. For instance, if a provider has no explicit mounthly cap on geocodes, but only allows 1 geocode per second, is it really true to describe that as 2.6 million geocodes per month? It would be extremely difficult in practice for any user to actually get anywhere near that.

### Links

* Live site: https://getlon.lat
