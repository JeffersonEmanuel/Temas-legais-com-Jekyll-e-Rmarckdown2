---
layout: post
title:  Correções de erros com htmlwidgets
date: 2017-07-18 16:11:49
published: true
tags: [htmlwidgets, r]
---

{% include htmlwidgets/__posts_include/ %}




<!--html_preserve--><div id="htmlwidget-260c19928c9a2ddece05" style="width:504px;height:504px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-260c19928c9a2ddece05">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"maxNativeZoom":null,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"continuousWorld":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":null,"unloadInvisibleTiles":null,"updateWhenIdle":null,"detectRetina":false,"reuseTiles":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addMarkers","args":[51.51895,-0.07125,null,null,null,{"clickable":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"Reasonably Priced Stella Artois",null,null,null,null,null,null]}],"limits":{"lat":[51.51895,51.51895],"lng":[-0.07125,-0.07125]}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->

Primeiro eu tive o seguinte erro:

!['highlight' tag was never closed](https://s12.postimg.org/cs1qm015p/erro_1.png)

Para corrigir, eu adicionei dentro do _config.yml a seguinte linha: **excerpt_separator: ""** 

Fazendo a correções acima o código execultor, mas o gráfico não apareceu. Ficou o seguinte erro:

![Erro ao apresentar o gráfico](https://s18.postimg.org/sghvs4tyx/erro_ao_apresentar_o_gr_fico.png)

Para corrigir este erro, primeiro adicionei as [dependencias]() no diretório raiz do projeto e o check no projeto .rmd: 

![](https://s17.postimg.org/z1us2nupb/check.png)

No diretório _includs criei um diretório chamado **htmlwidgets** e adicionei os .html dos posts lá dentro.










