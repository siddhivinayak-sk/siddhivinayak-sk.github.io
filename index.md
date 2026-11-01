---
layout: default
title: Sandeep Kumar
description: Open-source projects, practical engineering articles, and software architecture by Sandeep Kumar.
permalink: /
---

<style>
.site-footer .site-footer-credits {
  display: none !important;
}
</style>

{% include site-nav.html %}

<section class="profile-intro" aria-labelledby="intro-heading">
  <img class="profile-photo" src="{{ '/me-art.jpg' | relative_url }}" alt="Illustrated portrait of Sandeep Kumar">
  <div class="profile-intro-copy">
    <p class="eyebrow">Technical Architect · 16+ years of experience</p>
    <h1 id="intro-heading">Building thoughtful solutions for complex technology challenges.</h1>
    <p class="lead">I work across solution design, microservices, cloud platforms, and applied AI, with a focus on dependable software and secure delivery.</p>
    <p>I'm Sandeep Kumar, also known as <strong>Siddhivinayak-Sk</strong>. I believe open contribution and information sharing make technology more accessible and useful to everyone.</p>
    <p class="intro-links"><a class="button primary-button" href="{{ '/projects/' | relative_url }}">Explore open source <span aria-hidden="true">&rarr;</span></a><a class="button secondary-button" href="{{ '/writing/' | relative_url }}">Read my articles</a></p>
    <p class="intro-note"><a href="{{ '/profile/' | relative_url }}">Explore my experience</a> or <a href="{{ site.buymeacoffee_url | escape }}">support my work with a coffee</a>.</p>
  </div>
</section>

<section class="home-section" aria-labelledby="at-a-glance">
  <h2 id="at-a-glance">At a glance</h2>
  <ul class="highlights">
    <li><strong>Architecture & delivery</strong><span>From solution design and engineering through release and production support</span></li>
    <li><strong>Cloud & platforms</strong><span>Azure, AWS, GCP, Kubernetes, Docker, and Helm</span></li>
    <li><strong>AI engineering</strong><span>AI adoption, application integration, RAG, SFT, and agentic solutions</span></li>
    <li><strong>Industry experience</strong><span>BFSI, content, automotive, laboratory systems, eRetail, and learning</span></li>
  </ul>
</section>

<section class="home-section" aria-labelledby="selected-projects">
  <div class="section-heading"><h2 id="selected-projects">Built to be shared</h2><a href="{{ '/projects/' | relative_url }}">View all {{ site.data.projects | size }} projects <span aria-hidden="true">&rarr;</span></a></div>
  <p>Open-source tools and working examples for teams, testers, and engineers. Explore the code, try it out, or contribute.</p>
  {% assign featured_projects = site.data.projects | where: "featured", true %}
  {% include project-grid.html projects=featured_projects %}
</section>

<section class="home-section" aria-labelledby="selected-writing">
  <div class="section-heading"><h2 id="selected-writing">Ideas, explained through practice</h2><a href="{{ '/writing/' | relative_url }}">Browse all {{ site.data.articles | size }} articles <span aria-hidden="true">&rarr;</span></a></div>
  <p>Walkthroughs on cloud, security, developer tools, and software delivery, published on Medium.</p>
  {% assign featured_articles = site.data.articles | where: "featured", true %}
  {% include article-grid.html articles=featured_articles %}
</section>

{% include coffee-support.html %}

<section class="home-section contact-section" aria-labelledby="connect-heading">
  <h2 id="connect-heading">Connect</h2>
  <p>For professional details, visit my <a href="https://www.linkedin.com/in/siddhivinayak-sk">LinkedIn profile</a>. I also share work and ideas on:</p>
  <ul class="contact-links">
    <li><a href="https://github.com/siddhivinayak-sk">GitHub</a></li>
    <li><a href="https://siddhivinayak-sk.medium.com/">Medium</a></li>
    <li><a href="https://stackoverflow.com/users/4132230/sandeep-kumar">Stack Overflow</a></li>
    <li><a href="https://x.com/SiddhivinayakSk">X</a></li>
  </ul>
</section>
