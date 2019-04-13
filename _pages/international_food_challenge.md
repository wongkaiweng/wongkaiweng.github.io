---
permalink: "/international_food_challenge/"
---


## International Food Challenge!

{% for cuisine in site.international_food_challenge %}
  <li>
    <a class="post-link" href="{{ cuisine.url | prepend: site.baseurl }}">Cuisine {{ cuisine.cuisine }}</a>
  </li>
 {% include feature_row_posts feature_row= cuisine.feature_row %}

{% endfor %}

