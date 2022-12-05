---
permalink: /people/
title: "Members & Friends"
---

{% for people in site.people %}
  <p>
    <h5>{{ people.name }} - {{ people.committee_position }}</h5>
    {{ people.title}}
    <br>
    {{ people.org}}
  </p>
  <hr>
{% endfor %}