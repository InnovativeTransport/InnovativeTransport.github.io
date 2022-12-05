---
permalink: /events/
title: "Upcoming Events"
---

{% for event in site.events %}
  <p>
    <h4>{{ event.name}}</h4>
    <ul style="list-style:none">
      <li>When: {{ event.from_date | date_to_string }} - {{ event.to_date | date_to_string }} </li>
      <li>Where: {{ event.location }} </li>
      <li><a href="{{event.website}}">Website</a></li>
    </ul>
  </p>
  <hr>
{% endfor %}