---
layout: projects
title: Matteo Romiti's Projects
category: projects
---

- [Personal Reading List](https://matteoromiti.github.io/reading-list)
- [GitHub works:](https://github.com/MatteoRomiti)

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}
