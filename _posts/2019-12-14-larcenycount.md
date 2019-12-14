---
title: 'Explanatory analysis: Larceny count, San Francisco 2013-May 2018'
date: {}
published: true
tags:
  - dataviz
  - altair
  - hvplot
  - holoviews
excerpt: Embedding interactive charts on static pages using Jekyll.
hv-loader:
  hv-chart-1: charts/larceny count by year.html.html
  hv-chart-2: charts/larceny count by BG by year.html.html
toc: true
toc_sticky: true
---

## Hvplot - larceny count summarized by different groups
Firstly, larceny count can be summarized by years to see if the number of larcenies had a trend of growth or decrease in the past. For the analysis, we grouped the data by year and calculated the total number of incidents in each year. Then, we plotted a “step” plot for visualization.

In recent years (especially from 2012 to 2017), the number of larceny incidents continued increasing. Since we only got the data for first 5 months of 2018, the decrease from 2017 to 2018 in the graph is not useful for implication.
<div id="hv-chart-1"></div>

Secondly, larceny count can be summarized in each block group by years.To do this, we firstly converted the data with datetime parameters. Then we counted the number of incidents in each block group each year. After that, after getting the geometry of the block groups and converted the data to geodataframe, we conducted the visualization shown in the figure below. For example, in 2007, most larceny incidents happened in SOMA (south of Market street) and Union Square areas.
<div id="hv-chart-2"></div>

## Datashae - larceny count density
We got totally 480,448 larceny cases from the dataset and we visualized the preliminary view of the density of larceny incidents happened in San Francisco by using datashader package to aggregate the crime points and shade the aggregated pixels.

It is clear to notice that the northeastern part of the city (Chinatown, financial district and Tenderloin neighborhood) seems to have the highest density of larceny incidents in the past.
![Datashade_larcenydensity]({{ site.url }}{{ site.baseurl }}/assets/images/Datashade_larcenydensity.png)