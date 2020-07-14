---
layout: page
title: Warming Atlantic
short_name: warming_atlantic
permalink: viz/warming_atlantic
center_title: true
---

{% include small_table.html title="Tools" subtext="python, xarray, matplotlib, cartopy" %}

I really love the "[small multiples](https://www.displayr.com/what-are-small-multiples/)" approach in data visualization. I've also heard them called "postage stamp" plots. The idea is that you organize the same style of plot into a row-column format with some sort of change in each subplot. In climate science, it's most commonly used to illustrate change over time.

Here, I show the change in Atlantic Ocean sea surface temperatures from 1900 to 2017, relative to the 1890-1920 mean. Redder colors indicate warmer temperatures. You might notice in the later years a "[cold blob](https://en.wikipedia.org/wiki/Cold_blob_(North_Atlantic))" in the northern Atlantic near Greenland. This is an expected signal of anthropogenic climate change that could be due to the slowdown of the Atlantic Meridional Overturning Circulation (AMOC) and the injection of glacial meltwater, among other factors.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="/assets/img/viz/warming_atlantic/atlantic_small_multiples.jpg" alt=""/>
    </div>
</div>