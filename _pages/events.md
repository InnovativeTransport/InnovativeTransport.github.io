---
permalink: /events/
title: "Upcoming Events"
---

{% for event in site.events %}
  <h3>{{ event.name }}</h3>
  <p>{{ event.date | markdownify }} </p>
  <p>{{ event.location | markdownify }}</p>
  <p>{{ event.website | markdownify }}</p>
  <hr>
{% endfor %}