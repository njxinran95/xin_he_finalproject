---
title: "Explanatory analysis: Larceny count, San Francisco 2013-May 2018"
date: 2019-12-14
published: true
tags: [dataviz, altair, hvplot, holoviews]
excerpt: "Embedding interactive charts on static pages using Jekyll."
hv-loader:
  hv-chart-1: "charts/larceny count by year.html.html"
  hv-chart-2: "charts/larceny count by BG by year.html.html"
toc: true
toc_sticky: true
---

## Altair Example

Below is a chart of the incidence of measles since 1928 for the 50 US states.

This was produced using Altair and embedded in this static web page. Note that you can also display Python code on this page:

```python
import altair as alt
alt.renderers.enable('notebook')
```

## Holoviews Example

Lastly, the measles incidence produced using the Holoviews package:

<div id="hv-chart-1"></div>
<div id="hv-chart-2"></div>
![Datashade_larcenydensity]({{ site.url }}{{ site.baseurl }}/assets/images/Datashade_larcenydensity.png)
