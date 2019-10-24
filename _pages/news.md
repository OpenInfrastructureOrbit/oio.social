---
title: News
permalink: /news/
collection: news
show_excerpts: false
classes: wide
---
<ul>
    {% for item in site.news %}
    <li>
        <h2>{% if item.logo %}<img src="{{ item.logo }}" alt="Smiley face" height="42" width="42"> {% endif %} {{ item.date_time }} {{ item.title }}</h2>
        <p>{{ item.content | markdownify }}</p>
        {% if item.external_url %}
        <p><a href="{{ item.external_url }}" target="_blank" rel="noopener noreferrer">Weitere Informationen</a></p>
        {% endif %}
    </li>
    {% endfor %}
</ul>