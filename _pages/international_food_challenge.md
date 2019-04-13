---
permalink: "/international_food_challenge/"
layout: splash
title: International Food Challenge
excerpt: "**Indulge in a different cuisine every week**"
header:
  overlay_image: assets/images/international_food_challenge/header.jpg
  overlay_filter: rgba(0, 0, 0, 0.5)
---
Hi! This is where I record my challenge to cook a different cuisine every week.

:star: are the ones I would make again. Enjoy~

{% for cuisine in site.international_food_challenge %}
  <div>
    <b style= "color: rgb(255, 170, 170)" ><font size="18" style="color:rgb(128, 21, 21)">{{ cuisine.cuisine |upcase }}</font> Week {{cuisine.week_number}} ({{cuisine.week}}) </b>
  </div>
  <b style="color: rgb(212, 106, 106)">+++++++++++++++++++++++++++++++++++++++++++++++</b>

  **Important Ingredients**: {{cuisine.important_ingredients}}

  {{cuisine.notes}}

 {% include feature_row_4 feature_row= cuisine.feature_row %}

{% endfor %}

