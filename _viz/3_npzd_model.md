---
layout: page
title: NPZD Model
short_name: npzd_model
permalink: viz/npzd_model
center_title: true
---

{% include small_table.html title="Tools" subtext="python, javascript, bokeh, numpy" %}

One of the simplest ecosystem models one can make for an ocean model is a (N)utrient-(P)hytoplankton-(Z)ooplankton-(D)etritus model. It gets coupled to the ocean model physics to respond to things like solubility (temperature) changes, mixing, and upwelling. 

I wanted to make an interactive version of an NPZD model from an assignment in my Biogeochemical Oceanography class, based on the great [Sarmiento & Gruber textbook](https://press.princeton.edu/books/hardcover/9780691017075/ocean-biogeochemical-dynamics). Here I used `bokeh`, a package for making interactive python visualizations. You can move the sliders to play around with initial conditions and other parameters in the model.

This is a simple one-box model, so the generalized nutrient (which could be thought of as nitrate) is conserved. The top panel shows how the nutrient, phytoplankton, zooplankton, and detritus (zooplankton poop and dead phytoplankton) populations change over time. The bottom panel shows this in a different view, highlighting that the total nutrient is conserved.

The extended description and code can be found in my Jupyter notebook <a href="http://nbviewer.jupyter.org/github/bradyrx/Public-Notebooks/blob/master/NPZD-Model.ipynb">here.</a> You can view the full HTML page <a href="/assets/html/npzd_model.html">here</a>, if the inset on this page is difficult to navigate on your device.

<div>
<iframe src="/assets/html/npzd_model.html" width="100%" height="720">
</iframe>
</div>
