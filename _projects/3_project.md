---
layout: page
title: project 3
description: A Pipeline for Pre-Processing, Cleansing, and Visualizing AIS data with Ports Network Generation
img: assets/img/projects/ais-cruise-zoomed.png
importance: 3
category: work
---

During my M.Sc. at the University of Pisa, I had the opportunity to work as a visiting student at the Institute for Big Data Analytics at Dalhousie University. I worked on AIS data for cruise ships. After implementing a pipeline for pre-processing, cleansing, and generating ports network in Python for the ship data, I created a dashboard to visualize the Automatic Identification System (AIS) trajectories of vessels. Since these trajectories are characterized by a large number of points, efficiently visualizing them was important. To reach this goal, I simplified the polylines of trajectories by line simplification algorithm, Douglas-Peucker. Then, I plotted trajectories with different levels of detail. That is when zoomed out, a rough representation of trajectories is shown. By zooming in, the details are shown. I implemented this functionality by extending the Polyline class of Leaflet.js. When in a zoomed view, the number of points is less than a predefined threshold, the points of trajectories are shown. Otherwise, only the polylines are shown, and points are discarded.

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
