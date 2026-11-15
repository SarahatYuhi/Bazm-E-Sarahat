---
layout: home
title: Poet Name
---

<h2 class="intro">Selections from a life in verse</h2>
<p class="lead">A quiet collection of poems shaped by remembrance, longing, and the glow of love.</p>

<ul class="poem-list">
  {% for p in site.poems %}
    <li class="poem-item">
      <a href="{{ site.baseurl }}{{ p.url }}">
        <span class="title-roman">{{ p.title_roman }}</span>
        <span class="title-ur" lang="ur" dir="rtl">{{ p.title_ur }}</span>
      </a>
    </li>
  {% endfor %}
</ul>
