---
layout: page
title: Projects
published: false
---

The current research projects the the Autonomy and Verification Laboratory is involved in. Clicking the project's logo or picture will take you to the project's page or external website. This page also has information about our [Previous Projects](#previous-projects)

## Current projects
<br>

{% assign rows = site.projects.size | divided_by: 2.0 | ceil %}
{% for i in (1..rows) %}
<article class="row">
 {% assign offset = forloop.index0 | times: 2 %}
   {% for project in site.projects limit:2 offset:offset %}
      <section class="columns large-6">

          <h3> {{project.title}}</h3>
          <br>
          {{project.content}}

      </section>     
   {% endfor %}   
</article>
{% endfor %}




## Previous Projects

{% assign rows = site.projects-previous.size | divided_by: 2.0 | ceil %}
{% for i in (1..rows) %}
<article class="row">
 {% assign offset = forloop.index0 | times: 2 %}
   {% for project in site.projects-previous limit:2 offset:offset %}
      <section class="columns large-6">

          <h3> {{project.title}}</h3>
          <br>
          {{project.content}}

      </section>     
   {% endfor %}   
</article>
{% endfor %}
