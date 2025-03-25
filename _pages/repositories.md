---
layout: page
permalink: /repositories/
title: repositories
description: GitHub Repositories containing code accompanying papers, and/or functions that are useful
nav: true
nav_order: 5
---

{% if site.data.repositories.github_users %}



## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
