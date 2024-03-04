---
layout: page
title: Dynamic Population Estimation using Telecom Data
description: Graph Pattern-based Analysis of Call Detail Records Data for Dynamic Population Estimation
img: assets/img/projects/pisa_msc_1.jpg
importance: 1
category: work
related_publications: true
---

In this thesis project at the University of Pisa, I addressed the challenge of dynamic population estimation using telecommunication Call Detail Record (CDR) data as a valuable proxy for human mobility. CDRs are inherently noisy and contain numerous oscillations. In my thesis project, endeavored to identify these noise patterns, known as stationary-state noises, and eliminate them to render the data suitable for human mobility analysis.


Previous methodologies suggested density-based clustering of CDR locations and simply increasing the neighborhood distance if needed. Consequently, if a handoff occurs between two towers within the same cluster, it is deemed a spurious movement and categorized as a stop. I understood that this approach is not suitable for large areas covered by strong towers.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/florence-800m.png" title="clustering of tower locations" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Clustering of tower locations with DBSCAN e = 800 meters
</div>

My approach involved employing a graph pattern-based methodology to detect hand-off situations within a user's CDR data timeline. I selected a couple of noise patterns. Then, utilizing sequences of tower identifiers and connection times, I constructed mobility graphs and identified frequent noise patterns within them. These discovered patterns are then interpreted as stay locations within user trajectories.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/good_pattern1.png" title="Patterns in graphs" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/running_example_pisa.jpg" title="A CDR timeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Finding patterns in CDR timeline
</div>


Subsequently, stay locations serve as indicators of human presence and dynamic population across various spatial areas and temporal intervals. Additionally, I complemented my research with a visualization dashboard tailored for mobile phone data analysis, accommodating diverse filtering options across multiple data dimensions, and facilitating the application of different filters across multiple dimensions.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/dashboard.png" title="CDR Dashboard" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/pisa_msc_1.jpg" title="Dynamic Population" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Visualization Dashboard
</div>

The primary focus of my project was to dynamically estimate the population of census units. Furthermore, the refined data can be utilized to identify various events such as large gatherings, evacuations, and for transportation planning purposes.
