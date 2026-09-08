---
layout: default
title: Policy Unmaking
permalink: /journal/
---


<div class="journal-header">
  <img src="{{ '/assets/images/unmaking.png' | relative_url }}" alt="Policy Unmaking" class="journal-banner">
  <div class="journal-intro">
    <h1>Policy Unmaking</h1>
    <p style="font-size: 0.9rem;"> Half research digest, half (cynical) personal journal. Someone once said that policymaking is <em>a big pot that many stir</em>. Knowing who stirs it, what's in it and what the recipe is, helps us, citizens, understanding what we get on the plate. This blog tries to bring public policy theory in the everyday and discuss the recipes, the stakes and challenges of policymaking. It is largely based on research, my own and others' brilliant studies, but with more puns and less big words than academic writing often demands. You can also read it on <a href="https://giuseppec.substack.com/"> Substack</a></p>.
  </div>
</div>

<div class="journal-list">
  {% for post in site.posts %}
    <a href="{{ post.url | relative_url }}" class="journal-entry">
      <span class="journal-date">{{ post.date | date: "%B %d, %Y" }}</span>
      <h2>{{ post.title }}</h2>
      {% if post.excerpt %}
        <p class="journal-excerpt">{{ post.excerpt | strip_html | truncate: 140 }}</p>
      {% endif %}
    </a>
  {% endfor %}
</div>



