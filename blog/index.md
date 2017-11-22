---
layout: blog
title: Matteo Romiti's blog
category: blog
---

- What I think <br />
- What I learn <br />
- What I do

<hr>

<div class="blog-div">
  <ul class="blog-list">
    {% for post in site.posts %}
      <li class="blog-entry"><a href="{{ post.url }}"
      style="display:block;color:inherit;">
        <div class="blog-title">{{ post.title }}</div>
        <div class="post-excerpt">
        <p>
          <small><strong>{{ post.date | date: "%B %e, %Y" }} ~
          {% assign words = content | number_of_words %}
          {% if words < 360 %}
            1 min read
          {% else %}
            {{ words | divided_by:180 }} mins read
          {% endif %} <br />

          </strong></small>
          {{ post.excerpt | strip_html }}...
          </p>
        </div>
        </a>
      </li>
    {% endfor %}
  </ul>
</div>
