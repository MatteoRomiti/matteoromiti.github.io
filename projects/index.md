---
layout: projects
title: Matteo Romiti's Projects
category: projects
---

# Side Projects

{% for repository in site.github.public_repositories %}
  {% if repository.description contains '(Side' %}
* [{{ repository.name }}]({{ repository.html_url }}) <br />
  {{ repository.description }} <br />
  {{ repository.language }}
  {% endif%}
<!--     {{ repository.created_at }} -->
{% endfor %}

# Projects at Eurecom

{% for repository in site.github.public_repositories %}
  {% if repository.description contains 'Eurecom' %}
* [{{ repository.name }}]({{ repository.html_url }}) <br />
  {{ repository.description }} <br />
  {{ repository.language }}
  {% endif%}
<!--     {{ repository.created_at }} -->
{% endfor %}

# Projects at Polytechnic of Turin

{% for repository in site.github.public_repositories %}
  {% if repository.description contains 'Turin' %}
* [{{ repository.name }}]({{ repository.html_url }}) <br />
  {{ repository.description }} <br />
  {{ repository.language }}
  {% endif%}
<!--     {{ repository.created_at }} -->
{% endfor %}


