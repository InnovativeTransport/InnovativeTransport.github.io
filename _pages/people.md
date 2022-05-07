---
permalink: /people/
title: "Members & Friends"
---

{% for people in site.people %}
  <h3>{{ people.name }} - {{ people.committee_position }}</h3>
  <p>{{ people.org, people.title | markdownify }}</p>
{% endfor %}