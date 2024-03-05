---
layout: page
title: Social Network Analysis
description: Hashtag Co-occurrence Network during World Cup 2018
img: assets/img/projects/hashtag_2.png
importance: 3
category: work
---

The FIFA World Cup, often simply called the WorldCup, is an international football competition among different nations which is held once every four years. This event was one of the main highlighted sportive events during June and July 2018 and had so many fans and followers around the world. Twitter users are no exception and followed this event eagerly by tweeting about different topics including matches and events, using different hashtags. The main hashtag during this event was #WorldCup. Users appended this hashtag to their tweets along with some other hashtags and expressed their ideas. Also this event was a great opportunity for some of the users to express their off-topic ideas, including political, economical, cultural and environmental issues.


In this project, we study the various kinds of concerns raised by Twitter users, in terms of hashtags during the period of World Cup. We envisioned a network of hashtags, in which hashtags are related if they co- occur in a tweet and related hashtags are in clearly-cut communities. Since World Cup 2018 started from June 14, 2018, we collected all the tweets containing #WorldCup in the first week of the games (14th - 21st). Among different spelling variants, the hashtag #WorldCup had %81 of frequency and #worldcup had %16 of frequency1 . Thus, we also collected tweets containing #worldcup. For the first week, we gathered 1,809,545 tweets, containing #WorldCup or #worldcup.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/hashtag_1.png" title="Largest hubs in our crawled network" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/hashtag_2.png" title="Communities identified by Louvain" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Largest hubs in our crawled network. Communities identified by Louvain.
</div>


<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/hashtag_3.png" title="Degree Distribution of Our Hashtag Co-Occurence Network" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Degree Distribution of Our Hashtag Co-Occurence Network
</div>
