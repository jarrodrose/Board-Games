---
layout: home
title: "Board Game Resources"
---

## JR Owned
<ul>
{% for page in site.pages %}
  {% if page.layout contains 'game' %}
    {% if page.owned contains 'yes' %}
      <li><a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endif %}
{% endfor %}
</ul>

## Friends Owned or Wanted
<ul>
{% for page in site.pages %}
  {% if page.layout contains 'game' %}
    {% unless page.owned contains 'yes' %}
      <li><a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a></li>
    {% endunless %}
  {% endif %}
{% endfor %}
</ul>

## Links
- [BoardGameGeeks](https://boardgamegeek.com/) - Board game listing website
- [MechanicsBG](https://mechanicsbg.com/) - Website that explains board game mechanics
