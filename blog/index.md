---
layout: blog
title: Matteo Romiti's blog
category: blog
---

What I think, <br />
What I learn, <br />
What I do.

<hr>

<div class="blog-div">
  <ul class="blog-list">
    {% for post in site.posts %}
      <li class="blog-entry"><a href="{{ post.url }}"
      style="display:block;color:inherit;">
        <div class="blog-title">{{ post.title }}</div>
        <div class="post-excerpt">
        <p>
          {{ post.excerpt | strip_html }}...
          </p>
        </div>
        </a>
      </li>
    {% endfor %}
  </ul>
</div>
