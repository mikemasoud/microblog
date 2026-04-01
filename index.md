---
layout: default
title: Home
---

## Latest posts

{% for post in site.posts %}
<div class="post-card">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
  <p>{{ post.summary }}</p>
  <a class="read-more" href="{{ post.url }}">Read the full post</a>
</div>
{% endfor %}

<div class="about">
  <h2>About this micro blog</h2>
  <p>This micro blog publishes concise commentary and original analysis on governance, anti-corruption, internal control, ethical leadership, and institutional decision-making.</p>
  <p><strong>Author:</strong> Mike J. Masoud</p>
  <p><strong>Professional inquiries:</strong> <a href="mailto:info@theaaci.com">info@theaaci.com</a></p>
  <p><strong>Copyright:</strong> © 2026 Mike J. Masoud. All rights reserved.</p>
  <p><strong>Use of content:</strong> No part of this micro blog may be reproduced, republished, or redistributed without prior written permission, unless otherwise stated.</p>
</div>
