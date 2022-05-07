---
permalink: /people/
title: "Members & Friends"
---

{% for people in site.people %}
  <h2>{{ people.name }} - {{ people.committee_position }}</h2>
  <p>{{ people.org | markdownify }}, {{ people.title | markdownify }}</p>
{% endfor %}