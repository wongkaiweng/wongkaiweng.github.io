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



{% for cuisine in site.international_food_challenge %}
  <b>{{ cuisine.cuisine |capitalize }} - Week {{cuisine.week_number}} ({{cuisine.week}}) </b>
 {% include feature_row_4 feature_row= cuisine.feature_row %}

{% endfor %}

