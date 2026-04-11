---
layout: default
title: Categories
permalink: /categories/
---

<h1>Categories</h1>
<p class="categories-intro">Browse posts by topic.</p>

{% assign sorted_categories = site.categories | sort %}

{% for category in sorted_categories %}
  <section class="category-section">
    <h2 id="{{ category[0] | slugify }}">{{ category[0] | replace: '-', ' ' | capitalize }}</h2>
    <ul>
      {% assign posts = category[1] | sort: "date" | reverse %}
      {% for post in posts %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a>
          <small>— {{ post.date | date: "%B %-d, %Y" }}</small>
        </li>
      {% endfor %}
    </ul>
  </section>
{% endfor %}
