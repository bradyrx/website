---
layout: page
title: data visualization
nav_title: viz
description: static visualizations and movies
permalink: /viz/
nav: true
---

<section>
  <div class="thumb-container">
    {% for project in site.viz %}
      <a href="{{ site.url }}/{{ site.baseurl }}/{{ project.url }}">
        <div class="thumb-unit" 
             style="background-image: url({{ site.url }}/{{ site.baseurl }}/assets/img/viz/{{ project.short_name }}/thumb.jpg)">
          <div class="thumb-overlay">
            <strong>{{ project.title }} <i class="fa fa-arrow-right" aria-hidden="true"></i></strong>
          </div>
        </div>
      </a>
    {% endfor %}
  </div>
</section>
