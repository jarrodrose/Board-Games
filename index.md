---
layout: home
title: "Board Game Resources"
---

## JR Owned
- [Carcassonne](./games/carcassonne)
- [Catan](./games/settlers-of-catan)
- [Dixit: Disney Edition](./games/dixit-disney)
- [Munchkin](./games/munchkin)
- [Mysterium](./games/mysterium)
- [RoboRally](./games/roborally)

## Friends Owned
- [Dixit](./games/dixit)

## Links
- [BoardGameGeeks](https://boardgamegeek.com/) - Board game listing website
- [MechanicsBG](https://mechanicsbg.com/) - Website that explains board game mechanics

## Uncurated Page List
<ul>
{% for page in site.pages %}
  {% if page.layout contains 'game' %}
  	<li><a href="{{ page.url }}">{{ page.title }}</a></li>
  {% endif %}
{% endfor %}
</ul>
