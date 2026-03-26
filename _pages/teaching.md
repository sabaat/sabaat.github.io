---
layout: page
permalink: /teaching/
title: teaching
description: Courses taught as Graduate Teaching Assistant at Virginia Tech.
nav: true
nav_order: 6
calendar: false
---

I have been a **Graduate Teaching Assistant** at Virginia Polytechnic Institute and State University (Virginia Tech) since August 2022. Below are my teaching experience and the courses I have supported.

{% assign gtas = site.data.cv.cv.sections.Experience | where: "position", "Graduate Teaching Assistant" %}
{% if gtas and gtas.size > 0 %}
  <div class="card mt-3 p-3">
    <h3 class="card-title font-weight-medium">Teaching Experience</h3>
    {% assign entries = gtas %}
    {% include cv/experience.liquid %}
  </div>
{% endif %}

<div class="mt-4">
  <h3 class="card-title font-weight-medium">Courses</h3>
  {% include courses.liquid %}
</div>
