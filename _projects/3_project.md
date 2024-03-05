---
layout: page
title: project 3
description: A Pipeline for Pre-Processing, Cleansing, and Visualizing AIS data with Ports Network Generation
img: assets/img/projects/ais-cruise-zoomed.png
importance: 3
category: work
---

During my M.Sc. at the University of Pisa, I had the opportunity to work as a visiting student at the Institute for Big Data Analytics at Dalhousie University. I focused on AIS data for cruise ships. After developing a pipeline for preprocessing, cleansing, and generating a network of ports in Python for the ship data, I designed a dashboard to visualize the Automatic Identification System (AIS) trajectories of vessels. Given the high volume of points characterizing these trajectories, efficient visualization was crucial. To achieve this, I applied the Douglas-Peucker line simplification algorithm to simplify the polylines of trajectories. Subsequently, I plotted trajectories at various levels of detail. When zoomed out, a coarse representation of trajectories is displayed, while zooming in reveals finer details. I incorporated this functionality by extending the Polyline class of Leaflet.js. Specifically, when in a zoomed-out view and the number of points falls below a predefined threshold, the trajectory points are displayed. Otherwise, only the polylines are shown, and the points are discarded.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/ais-dashboard.png" title="Dashboard" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/ais-cruise-zoomed.png" title="Zoomed view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Dashboard with the Ports Network and speed distribution chart. Zoomed view with points revealed.
</div>
