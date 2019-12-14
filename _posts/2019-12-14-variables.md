---
title: 'Explore predicted and explanatory variables'
date: 2019-12-14
published: true
tags:
  - dataviz
  - altair
  - hvplot
  - holoviews
excerpt: Explanatory analysis of predicted and explanatory variables, including static images produced by Seabon and Matplotlib.
toc_sticky: true
---
## Predicted variable: Larceny index
The Larceny Index for a block group would be equal to **total number of larceny incidents divided by total population in the block group and then times 100,000.**

From the histogram of actual larceny index as below, most block groups have larceny index less than 500,000, there are some over 1 million, the maximum even reaches to 6,000,000.
![hist-larceny index]({{ site.url }}{{ site.baseurl}}/assets/images/hist-larceny index.png)

## Explanatory variables

### Correlation of all explanatory variables
The absolute values of all correlation indexes are smaller than 0.8, so we considered that all explanatory variables could be included in our model.
![Correlation among variables]({{ site.url }}{{ site.baseurl}}/assets/images/Correlation among variables.png)

### Pairplots
We used **pairplots** to show the relations between explanatory variables in detail. In this step, we produced the pairplots based on the general categories: demographic, housing, land use, and 311-related.

**1. Pairplot of demographic data**
![Pairplot-Demo]({{ site.url }}{{ site.baseurl}}/assets/images/Pairplot-Demo.png)

**2. Pairplot of housing data**
![Pairplot-Housing]({{ site.url }}{{ site.baseurl}}/assets/images/Pairplot-Housing.png)

**3. Pairplot of land use data**
![Pairplot-Land use]({{ site.url }}{{ site.baseurl}}/assets/images/Pairplot-Land use.png)

**4. Pairplot of 311-related data**
![Pairplot-311]({{ site.url }}{{ site.baseurl}}/assets/images/Pairplot-311.png)

As the above pairplots show, in each general category, there are no two explanatory variables which have obvious linear relationship to each other. Thus, it proves that all explanatory variables could be included in the model without worrying about multicollinearity.
