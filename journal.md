---
layout: default
title: Policy Unmaking
permalink: /journal/
---


<div class="journal-header">
  <img src="{{ '/assets/images/fieldnotes.png' | relative_url }}" alt="Policy Unmaking" class="journal-banner">
  <div class="journal-intro">
    <h1>(unful)fieldwork</h1>
    <p style="color: #FFCE19; font-weight: 600;"> Research notes and ramblings </p>


  <p style="font-size: 0.9rem;"> Research is a weird kind of job. In my line of work, public policy research – or, as my uncle would call it, a waste of public funds – you are expected to know stuff. That's your job, studying, learning, knowing things. It's a debatable reason for getting a salary, but I would not be the one raising this objection. Fieldwork, is a big part of this job. I follow people, what they do, with a set of assumptions about how policy is being made, and ask them how and why they do what they do. I record my interviews or jot down my notes and watch those assumption crumble, question after question. So, I go back to reflect on my failures, and I read, read, and read again about all the interesting things very smart people have written over the past decades. I work out a couple of slightly sharper, brand-new interpretations, I get face to face with my interviewees and watch them proving me wrong again. So, I roll up my sleeves and… well, you get it at this point.</p>
    
  <p style="font-size: 0.9rem;"> This process, I came to realise, is not necessarly a waste of time. One of the things I have learned over the past few years, is that to understand how something works, get a somewhat truthful interpretation of what is going on, you need to dwell. To stay with your topic, your objects of study, and – crucially – your thoughts. I believe that research, at least the kind of research I do, requires this dwelling, pondering, doubting what you see and yourself. As a chronically anxious and self-doubting person, I have spent a lot of time with my thoughts as a researcher that I know may have a few things to say about (at least) my reseach practice, methods, and the role of the research in this broader picture. This is what this blog is about.
    
  Occasionally, I plan to publish some of my ramblings also in research-based ramblings about how policy theories can be useful to think about our present in my unsystematic sort of newsletter, <a href="https://giuseppec.substack.com/"> Policy Unmaking</a>, on Substack.</p>
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



