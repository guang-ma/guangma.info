---
layout: page
permalink: /repositories/
title: data & code
description: # data & code repositories used in my publications.
nav: true
nav_order: 4
---

Disclaimer: You may download the data and programming codes for your research/teaching use. The data is provided as is. I would appreciate it if you make proper acknowledgements in your work. If you find any errors in the data and codes, please feel free to inform me. Thanks!

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
