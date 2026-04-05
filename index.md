---
layout: default
title: Home
---

## Latest posts

{% for post in site.posts %}
<div class="post-card">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
  <p><strong>Summary:</strong> {{ post.summary }}</p>
  <p><strong>Why it matters:</strong> {{ post.why_it_matters }}</p>
  <a class="read-more" href="{{ post.url }}">Read the full post</a>
</div>
{% endfor %}

<div class="about">
  <h2>About this micro blog</h2>
  <p>This micro blog publishes concise commentary and original analysis on governance, anti-corruption, internal control, ethical leadership, and institutional decision-making.</p>
  <p><strong>Author:</strong> Mike J. Masoud</p>
  <p><strong>Professional inquiries:</strong> <a href="mailto:info@theaaci.com">info@theaaci.com</a></p>
  <p><strong>Copyright:</strong> © 2026 Mike J. Masoud. All rights reserved.</p>
</div>

<div class="explore-more">
  <h2>Explore more</h2>
  <p>Readers interested in additional analysis, commentary, and practical engagement can also explore the following:</p>
  <p><strong><a href="https://www.linkedin.com/newsletters/the-aaci-dispatch-7321647166328827904/" target="_blank" rel="noopener noreferrer">The AACI Dispatch on LinkedIn</a></strong> — A monthly newsletter featuring analysis, commentary, and insights on anti-corruption, governance, and institutional integrity.</p>
  <p><strong><a href="https://theaaci.substack.com" target="_blank" rel="noopener noreferrer">Power &amp; Accountability on Substack</a></strong> — A publication exploring deeper perspectives on corruption prevention, ethical leadership, accountability, and institutional risk.</p>
  <p><strong><a href="https://certification.theaaci.com/aaci-assistant" target="_blank" rel="noopener noreferrer">The AACI Assistant</a></strong> — An interactive assistant designed to help readers explore AACI-related anti-corruption concepts, ideas, and resources.</p>
</div>
