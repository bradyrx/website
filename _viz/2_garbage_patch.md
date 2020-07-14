---
layout: page
title: Great Pacific Garbage Patch
short_name: garbage_patch
permalink: viz/garbage_patch
center_title: true
---

{% include small_table.html title="Tools" subtext="ParaView, python, Fortran" %}
{% include small_table.html title="Awards" subtext="Runner-Up, NASA Data Visualization and Storytelling Competition" %}


The Great Pacific Garbage Patch is a massive patch of microplastics [twice the size of Texas](https://www.usatoday.com/story/tech/science/2018/03/22/great-pacific-garbage-patch-grows/446405002/). In working with a simulation I ran of the Los Alamos National Lab's Model for Prediction Across Scales–Ocean (MPAS–O), I accidentally recreated the garbage patch. See my page on [Southern Ocean Carbon](/viz/southern_ocean_carbon) for details on the simulation.

I created the video below in Paraview, which shows the evolution of surface particles over 17 years of simulation. You can imagine these surface particles as microplastics. Note that this isn't what it would look like from space, since these microplastics are extremely tiny. The cool thing about this simulation is you can see how gyre circulation in the North Pacific naturally gathers surface particles into a collected mass. This is largely due to a process called [Ekman transport](https://www.open.edu/openlearn/science-maths-technology/the-oceans/content-section-4.4), which causes waters (and things suspended in those waters) to converge at the center of gyres.

<iframe src="https://player.vimeo.com/video/357112846" width="640" height="360" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>
<p><a href="https://vimeo.com/357112846">The Great Pacific Garbage Patch</a> from <a href="https://vimeo.com/user96067365">Riley Brady</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

This video was a part of the package I submitted to the [NASA Data Visualization and Storytelling Competition](https://education.agu.org/grants/data-visualization-storytelling-competition/), in which a team of myself, Annie Bares (UT Austin), and Stephanie Zeller (UT Austin) were runners-up. An earlier iteration is one of the top all-time posts on the subreddit [/r/dataisbeautiful](https://old.reddit.com/r/dataisbeautiful/comments/cvoyti/the_great_pacific_garbage_patch_oc/) and generated some lively discussion. It was also covered on [Digg](https://digg.com/2019/the-great-pacific-garbage-patch-visualized), among other sites. This work was also featured on the [cover](/assets/pdf/IEEE_CG_cover.pdf) of the <i>IEEE Computer Graphics and Applications</i> magazine with a [feature story](/assets/pdf/KillingRainbows.pdf).