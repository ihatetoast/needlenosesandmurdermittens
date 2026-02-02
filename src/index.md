---
layout: base.njk
title: Needle Noses and Murder Mittens
---

# Needle Noses and Murder Mittens

{% for post in collections.all %}

<article>
  <h2>
    <a href="{{ post.url}}" >{{ post.data.title }}</a>
  </h2>
{% if post.data.image %}
 <img  src="{{post.data.image}}" alt="{{post.data.title}}" width="400"/>
{% endif %}
</article>

{% endfor %}
