---
layout: default
title: Projects | Sandeep Kumar
description: Open-source tools and examples for agile teams, AI risk validation, JMeter, Azure, Kubernetes, and application security.
permalink: /projects/
---

{% include site-nav.html %}

<header class="page-intro">
  <p class="eyebrow">Open source / practical engineering</p>
  <h1>Tools to use. Code to explore. Ideas to build on.</h1>
  <p class="lead">I share practical solutions across AI, cloud, identity, testing, and microservices. Each project is an invitation to learn, experiment, and contribute.</p>
  <a class="button primary-button" href="https://github.com/siddhivinayak-sk?tab=repositories">Browse all repositories on GitHub <span aria-hidden="true">&rarr;</span></a>
</header>

{% assign project_groups = site.data.projects | group_by: "category" %}
<nav class="topic-nav" aria-label="Project categories">
  {% for group in project_groups %}
  <a href="#{{ group.name | slugify }}">{{ group.name | escape }}</a>
  {% endfor %}
</nav>

{% for group in project_groups %}
<section class="catalog-section" aria-labelledby="{{ group.name | slugify }}">
  <div class="section-heading">
    <h2 id="{{ group.name | slugify }}">{{ group.name | escape }}</h2>
    <span class="section-count">{{ group.items | size }} projects</span>
  </div>
  {% include project-grid.html projects=group.items %}
</section>
{% endfor %}

<p class="catalog-note">Looking for a walkthrough? Explore my <a href="{{ '/writing/' | relative_url }}">technical articles</a> for related explanations and examples.</p>

{% include coffee-support.html %}
