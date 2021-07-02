---
title: BlockDB
subtitle: A curated list of cryptocurrency resources.
layout: layouts/base.njk
---


{% for listing in db %}

<div class="listing-content">
  <div class="listing-info">
    <p class="listing-name">{{ listing.name }}</p>
    <span class="listing-description">{{ listing.description }}</span>
    <div class="listing-image">
    <img src="{{ listing.image }}" width="20%"/>
    </div>
    <div class="button">
      <span style="color:#fc8812">Visit</span>
      <img src="/images/arrow.svg" style="filter:invert(56%) sepia(98%) saturate(700%) hue-rotate(352deg) brightness(107%) contrast(98%);" alt="External link arrow">
    </div>
  </div>
  <div class="listing-resources">
  <div class="listing-resource-item">
    {% if listing.blog %}<span><img src="/images/align-left.svg" height="100%"></span>{% endif %}
    {% if listing.blog %}<span><a class="resource-name" href="{{ listing.blog }}">Blog</span>{% endif %}
  </div>
  <br>
  <div class="listing-resource-item">
    {% if listing.github %}<span><img src="/images/terminal.svg" height="100%"></span>{% endif %}
    {% if listing.github %}<span><a class="resource-name" href="{{ listing.github }}">GitHub</span>{% endif %}
  </div>
  <ul>
    {% if listing.blog %}<li><a href="{{ listing.blog }}">Blog</li>{% endif %}
    {% if listing.etherscan %}<li><a href="{{ listing.etherscan }}">Etherscan</li>{% endif %}
    {% if listing.github %}<li><a href="{{ listing.github }}">GitHub</li>{% endif %}
  </ul>
  </div>
</div>

{% endfor %}
