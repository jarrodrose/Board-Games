---
layout: home
title: "Board Game Resources"
---

## My Collection
<ul>
{% for game_file in site.data.games %}
  {% assign game = game_file[1] %}
  {% if game.owned %}
    <li><a href="{{ site.baseurl }}/games/{{ game_file[0] }}">{{ game.title }}</a></li>
  {% endif %}
{% endfor %}
</ul>

## Wishlist
<ul>
{% for game_file in site.data.games %}
  {% assign game = game_file[1] %}
  {% unless game.owned %}
    <li><a href="{{ site.baseurl }}/games/{{ game_file[0] }}">{{ game.title }}</a></li>
  {% endunless %}
{% endfor %}
</ul>

## Links
- [BoardGameGeeks](https://boardgamegeek.com/) - Board game listing website
- [MechanicsBG](https://mechanicsbg.com/) - Website that explains board game mechanics
