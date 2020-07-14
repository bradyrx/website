---
layout: page
title: Adventure Map
short_name: adventure_map
permalink: viz/adventure_map
center_title: true
---

{% include small_table.html title="Tools" subtext="python, gpxpy, mplleaflet" %}

I use a Garmin Forerunner GPS watch when running, hiking, and cycling. I started using it while running to track my mileage through <a href="https://www.strava.com/athletes/17249172">Strava</a>, but then realized I could manually view and manipulate the GPX files. 

For one, I could tweak the GPX files to make myself look faster. But I decided to spend my time making an interactive map of all the places the watch has tracked me working out and exploring. This can be construced pretty easily with the python packages `gpxpy` and `mplleaflet`. You can check out the code <a href="https://github.com/bradyrx/run_and_ride_map/blob/master/gpx_play.ipynb">here</a>.


You'll notice various coloring of the lines on the map. <font color="red">Red</font> denotes running, <font color="purple">purple</font> cycling, and <font color="brown">brown</font> hiking. Note that this map is a few years out of date. Strava changed the way they archive your files, so I haven't been able to get access again to the raw GPX files.

You can view the full map in your browser [here](/assets/html/adventure_map.html).

<div>
<iframe src="/assets/html/adventure_map.html" width="100%" height="720">
</iframe>
</div>
