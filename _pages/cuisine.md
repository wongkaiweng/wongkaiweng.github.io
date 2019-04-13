---
permalink: "/cuisine/"

---
## International Food Challenge!

{% for cuisine in site.cuisine %}
  <li>
    <a class="post-link" href="{{ cuisine.url | prepend: site.baseurl }}">Cuisine {{ cuisine.cuisine }}</a>
  </li>
{% endfor %}

