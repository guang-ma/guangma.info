---
layout: page
permalink: /data/
title: data & code
description: # data & code repositories used in my publications.
nav: true
nav_order: 3
---

Disclaimer: You may download the data and programming codes for your research/teaching use. The data is provided as is. I would appreciate it if you make proper acknowledgements in your work. If you find any errors in the data and codes, please feel free to inform me. Thanks!

<div class="row">
      <div class="col-sm-9">
        <h3>TPP--Technological Peer Pressure</h3>
      <p>The variable 'TPP' proposed by Cao, Ma, Tucker, and Wan (2018), <a href ="https://doi.org/10.2308/accr-52056">'Technological Peer Pressure and Product Disclosure'</a>, The Accounting Review, Vol 93 (6), pp 95-126. </p>
      <p>The data file contains the TPP measure for Compustat firms for fiscal years 1990-2019, in Stata .dta format.</p>
      <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
      {% include repository/repo.liquid repository='guang-ma/tpp' %} 
      </div>
</div>

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
