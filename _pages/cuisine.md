---
permalink: "/cuisine/"
---


## International Food Challenge!

{% for cuisine in site.cuisine %}
  <li>
    <a class="post-link" href="{{ cuisine.url | prepend: site.baseurl }}">Cuisine {{ cuisine.cuisine }}</a>
  </li>
  HELLO
  {% include feature_row_posts feature_row= cuisine.feature_row %}

{% endfor %}


