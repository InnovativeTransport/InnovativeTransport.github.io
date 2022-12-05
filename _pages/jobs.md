---
permalink: /jobs/
title: "Job Postings"
---

{% for jobs in site.jobs %}
  <p>
    <h4>{{ jobs.organization }} - {{ jobs.title }}</h4>
    {{ jobs.description}}
    <br>
    <a href="{{ jobs.link}}">Posting</a>
  </p>
  <hr>
{% endfor %}