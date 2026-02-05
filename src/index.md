---
layout: base.njk
title: Needle Noses and Murder Mittens
---

{% for post in collections.posts %}

  <article class="main-page-article">
    <h2 class="post-data-title">
      <a href="{{ post.url }}">{{ post.data.title }}</a>
    </h2>
    {% if post.data.image %}
      <div class="main-page-image-container">
        <img src="{{ post.data.image }}" alt="{{ post.data.title }}" />
      </div>
    {% endif %}
  </article>

{% endfor %}