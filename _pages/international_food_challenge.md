---
permalink: "/international_food_challenge/"
layout: splash
title: International Food Challenge
excerpt: "**Indulge in a different cuisine every week**"
header:
  overlay_image: /assets/images/unsplash-image-1.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  actions:
    - label: "More Info"
      url: "https://unsplash.com"
---
:star: are the ones I would make again.

{% for cuisine in site.international_food_challenge %}
  <div style="background-color: rgb(212, 106, 106)">
    <b style= "color: rgb(255, 170, 170)" ><font size="18" style="color:rgb(128, 21, 21)">{{ cuisine.cuisine |upcase }}</font> Week {{cuisine.week_number}} ({{cuisine.week}}) </b>
  </div>
  **Important Ingredients**: {{cuisine.important_ingredients}}

  {{cuisine.notes}}

 {% include feature_row_4 feature_row= cuisine.feature_row %}

{% endfor %}

