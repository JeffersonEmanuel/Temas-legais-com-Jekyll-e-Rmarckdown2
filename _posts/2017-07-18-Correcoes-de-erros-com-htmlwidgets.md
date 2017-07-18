---
layout: post
title:  Correcoes-de-erros-com-htmlwidgets
date: 2017-07-18 13:45:58
published: true
tags: [htmlwidgets, r]
---







{% highlight r %}
library(leaflet)

m <- leaflet() %>%
  addTiles() %>%  # Add default OpenStreetMap map tiles
  addMarkers(lng = -0.07125, lat = 51.51895, 
             popup = "Reasonably Priced Stella Artois")
m
{% endhighlight %}



{% highlight text %}
## Error in loadNamespace(name): there is no package called 'webshot'
{% endhighlight %}


















