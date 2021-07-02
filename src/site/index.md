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
    <br>
    <div class="button">
      <span style="color:#fc8812">Visit</span>
      <img src="/images/arrow.svg" style="filter:invert(56%) sepia(98%) saturate(700%) hue-rotate(352deg) brightness(107%) contrast(98%);" alt="External link arrow">
    </div>
  </div>
  <div class="listing-img">
    <img src="{{ listing.image }}" width="100%" style="border-radius:0.2rem"/>
    </div>
</div>

{% endfor %}
