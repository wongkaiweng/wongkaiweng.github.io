---
permalink: "/international_food_challenge/"
---
## International Food Challenge!

<ul>
  {% for cuisine in site.interional_food_challenge %}
    <li>
      <a href="{{ cuisine.url }}">{{ cuisine.title }}</a>
      - {{ cuisine.headline }}
    </li>
  {% endfor %}
</ul>

