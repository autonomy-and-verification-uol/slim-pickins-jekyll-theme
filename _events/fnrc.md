---
layout: event
title: "Future of Nuclear Robotics Certification Workshop Series"
series : true
published: false
---

<div class="row" >
  <div class="columns large-4" >
    <img alt="University of Liverpool logo" style="float: left; width : 22em; margin-bottom : 2em " src="{{site.images}}logos/UoL.png">
    <img alt="RAIN Hub logo" style="float: left; width : 15em; " src="{{site.images}}logos/rain-logo.png">
  </div>

  <div class="columns large-8" markdown="1">

A series of workshops, organised by researchers at the University of <a href="({{site.UoL_URL}})" alt="Universtiy of Liverpool Computer Science Department"> Liverpool</a>, linked to our work with the <a href="{{site.url}}/projects/rai-hubs" alt="Robotics and Artificial Intelligence Hubs project page">Robotics and Artificial Intelligence Hubs</a>. These workshops tackle the current and emerging safety justification issues that autonomous and robotic systems raise in the nuclear industry. These workshops will introduce certification challenges (using safety cases, providing certification evidence, etc) across the nuclear estate.

## Mailing List

If you would like to keep up to date with the workshop series and its outputs you can sign up to our <a href="https://www.jiscmail.ac.uk/FNRC-WORKSHOPS" alt="Workshop's Mailing List Link">mailing list.</a> We will use this to announce new workshops and to communicate the workshops output.

 </div>
 </div>


## Workshops
<ul>
{% for event in site.events  %}
{% if event.belogsToSeries contains 'fnrc' %}
<li> [{{ event.date | date: "%-d %B %Y" }}] <a href="{{site.url}}{{event.url}}" alt="{{event.title}}"> {{event.title}} </a>  </li>
{% endif %}
{% endfor %}
</ul>
