---
layout: default
title: Policy Unmaking
permalink: /journal/
---


<div class="journal-header">
  <img src="{{ '/assets/images/unmaking.png' | relative_url }}" alt="Policy Unmaking" class="journal-banner">
  <div class="journal-intro">
    <h1>Policy Unmaking</h1>
    <p style="font-size: 0.8rem;">Half research digest, half cynical personal journal. Someone once said that policymaking is a big pot that many stir. Knowing who stirs it, what's in the pot and what recipes is being follew helps us understanding what we get on the plate. Unpaking this recipes, is the goal of this blog, which tries to combine research and the everyday, with a public policy theory twist. </p>
  </div>
</div>

<div class="journal-list">
  {% for post in site.posts %}
    <a href="{{ post.url | relative_url }}" class="journal-entry">
      <span class="journal-date">{{ post.date | date: "%B %d, %Y" }}</span>
      <h2>{{ post.title }}</h2>
      {% if post.excerpt %}
        <p class="journal-excerpt">{{ post.excerpt | strip_html | truncate: 200 }}</p>
      {% endif %}
    </a>
  {% endfor %}
</div>



