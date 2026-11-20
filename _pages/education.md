---
layout: archive
title: "Education Packages"
permalink: /education/
author_profile: true
---

{% include base_path %}

Quantum computing is often seen as hard to get into, but its core ideas can be explained simply. Each package below takes one concept from my research and explains it in a few minutes, using an everyday analogy, a picture, and a small worked example. Every package states who it is for and what you need to know beforehand.

{% for post in site.education %}
  {% include archive-single.html %}
  {% if post.audience %}<p class="page__meta"><strong>For:</strong> {{ post.audience }} · <strong>Level:</strong> {{ post.level }} · <strong>Time:</strong> {{ post.duration }}</p>{% endif %}
{% endfor %}
