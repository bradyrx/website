---
layout: page
title: Southern Ocean Carbon
short_name: southern_ocean_carbon
permalink: viz/southern_ocean_carbon
center_title: true
---

{% include small_table.html title="Tools" subtext="ParaView, python, Fortran" %}
{% include small_table.html title="Awards" subtext="Runner-Up, NASA Data Visualization and Storytelling Competition" %}


As a part of my [Department of Energy Computational Science Graduate Fellowship](https://www.krellinst.org/csgf/fellows/profile?n=brady2016), I spent a summer at Los Alamos National Lab running simulations of their global ocean model. It's called the [Model For Prediction Across Scales–Ocean](https://mpas-dev.github.io/ocean/ocean.html) (MPAS-O), and it's super cool.

The majority of climate models use [rectilinear or curvilinear meshes](https://en.wikipedia.org/wiki/Regular_grid), which create discrete grid cells by drawing straight or curved lines over the Earth's surface like a tic-tac-toe board. Instead, MPAS–O uses an "unstructed" mesh of hexagons. This allows one to vary the size of hexagons in important areas of interest–such as coastlines–while keeping larger hexagons in other areas of the ocean to save computational expense.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="/assets/img/viz/southern_ocean_carbon/hex_mesh.png" alt=""/>
    </div>
</div>
<div class="caption">
    The MPAS–O model mesh. From Petersen et. al (2019), <i>JAMES</i>.
</div>

In the simulations I ran, we used what's called a Lagrangian particle tracking system. Specifically, we used code called [LIGHT](https://pwolfram.github.io/light/) written by one of my Los Alamos advisors, [Phil Wolfram](pwolfram.github.io). The classical view of a climate model is Eulerian in nature. In this framework, we grid the Earth into discrete cells (in this case hexagons) and solve Partial Differential Equations (PDEs) of fundamental fluid physics, stepping forward in time. This method produces a single value for each grid cell at each time step for a suite of variables: things like temperature, salinity, sea surface height, dissolved carbon, and nutrients. However, these grid cells are hundreds of kilometers on each side. The temperature or dissolved carbon in a given grid cell is the result of myriad processes, such as mixing, air-sea exchange, biology, and upwelling. By using the Lagrangian framework, it's as if we drop a bunch of autonomous submarines in the water that track how individual water parcels flow. Or if we were to drop [thousands of rubber ducks at sea](https://www.npr.org/2011/03/29/134923863/moby-duck-when-28-800-bath-toys-are-lost-at-sea) to watch how the currents flow.

The results of such a simulation are stunning.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="/assets/img/viz/southern_ocean_carbon/thumb.jpg" alt=""/>
    </div>
</div>
<div class="caption">
    Trajectories of surface floats over one month of simulation in MPAS–O. They are colored by the temperature they record every two days. Each line follows a single float's path.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="/assets/img/viz/southern_ocean_carbon/carbon_iris.jpg" alt=""/>
    </div>
</div>
<div class="caption">
    Trajectories of all floats over one month of simulation in MPAS–O. They are colored by the dissolved inorganic carbon they record every two days. Each line follows a single float's path. Bluer colors near Antarctica denote enriched dissolved inorganic carbon driven by respiration of dead organic matter at depth and its subsequent curl-driven upwelling to the surface.
</div>

While static images are nice, I think you can really get intuition for how carbon flows around the ocean with some movies. To make these videos, I used Paraview, an open-source visualization application. In the first video, I show carbon flowing between 500 m and 3,000 m depth. The trajectories are colored by their carbon content, where the yellow colors are carbon-deplete (toward the surface) and purple colors carbon-enriched (toward depth).

<iframe src="https://player.vimeo.com/video/365579177" width="640" height="360" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>
<p><a href="https://vimeo.com/365579177">The Flow of Dissolved Carbon in the Southern Ocean</a> from <a href="https://vimeo.com/user96067365">Riley Brady</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

This video is similar, but I was experimenting with a rotating view around the Southern Ocean. The land mass on top is Antarctica, and you can see individual floats move around on the surface.

<iframe src="https://player.vimeo.com/video/337393622" width="640" height="512" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>
<p><a href="https://vimeo.com/337393622">Surface BGC Floats in MPAS Ocean</a> from <a href="https://vimeo.com/user96067365">Riley Brady</a> on <a href="https://vimeo.com">Vimeo</a>.</p>
