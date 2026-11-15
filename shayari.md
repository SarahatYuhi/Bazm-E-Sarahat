---
layout: category
title: Shayari
permalink: /shayari/
---

<ul class="category-list">
  {% assign shayari_items = site.poems | where_exp: 'item', 'item.path contains "/shayari/"' %}
  {% for item in shayari_items %}
    <li class="category-item">
      <a href="{{ site.baseurl }}{{ item.url }}">
        <span class="title-roman">{{ item.title_roman }}</span>
        <span class="title-ur" lang="ur" dir="rtl">{{ item.title_ur }}</span>
      </a>
    </li>
  {% endfor %}
</ul>
