---
layout: page
title: Blog
---

<div class="post-list">

  {% for post in site.posts %}
    <article class="post-list-item">

      <h2>
        <a href="{{ post.url | relative_url }}">
          {{ post.title }}
        </a>
      </h2>

      <time datetime="{{ post.date | date_to_xmlschema }}">
        วันที่โพส {{ post.date | date: "%d/%m/%Y" }}
      </time>

    </article>
  {% endfor %}

</div>