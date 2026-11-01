---
layout: default
title: Writing | Sandeep Kumar
description: Practical Medium articles on cloud, Kubernetes, developer tools, authentication, application architecture, and DevOps.
permalink: /writing/
---

{% include site-nav.html %}

<header class="page-intro">
  <p class="eyebrow">Writing / learning in the open</p>
  <h1>From an engineering question to a working example.</h1>
  <p class="lead">My articles unpack cloud platforms, application architecture, identity, and software delivery through practical guides and technical walkthroughs.</p>
  <a class="button primary-button" href="https://siddhivinayak-sk.medium.com/">Follow my writing on Medium <span aria-hidden="true">&rarr;</span></a>
</header>

{% assign article_groups = site.data.articles | group_by: "category" %}
<nav class="topic-nav" aria-label="Article topics">
  {% for group in article_groups %}
  <a href="#{{ group.name | slugify }}">{{ group.name | escape }}</a>
  {% endfor %}
</nav>

{% for group in article_groups %}
<section class="catalog-section" aria-labelledby="{{ group.name | slugify }}">
  <div class="section-heading">
    <h2 id="{{ group.name | slugify }}">{{ group.name | escape }}</h2>
    <span class="section-count">{{ group.items | size }} articles</span>
  </div>
  {% include article-grid.html articles=group.items %}
</section>
{% endfor %}

<p class="catalog-note">Prefer to dive into the code? Browse my <a href="{{ '/projects/' | relative_url }}">open-source projects</a>. For more articles and updates, visit <a href="https://siddhivinayak-sk.medium.com/">my Medium profile</a>.</p>

{% include coffee-support.html %}
