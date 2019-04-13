---
permalink: "/international_food_challenge/"
layout: splash
---


## International Food Challenge!

{% for cuisine in site.international_food_challenge %}
  <b>{{ cuisine.cuisine |capitalize }} - Week {{cuisine.week_number}} ({{cuisine.week}}) </b>
 {% include feature_row_4 feature_row= cuisine.feature_row %}

{% endfor %}

