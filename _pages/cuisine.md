---
permalink: "/cuisine/"

---
## International Food Challenge!

<h1>Chapters</h1>

<ul class="posts">
{% for cuisine in site.cuisine %}
  <li>
    <a class="post-link" href="{{ cuisine.url | prepend: site.baseurl }}">Cuisine {{ cuisine.cuisine }}</a>
  </li>
{% endfor %}
</ul>

