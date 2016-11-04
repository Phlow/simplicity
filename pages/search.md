---
layout: page
title: "Search"
permalink: /search/
sitemap: false
---
{% include search %}

<h2>{{ site.language.search_results }}</h2>

<ul id="search-results" class="toc"></ul>

<script>
  window.store = {
    {% for post in site.posts %}
      "{{ post.url | slugify }}": {
        "title": "{{ post.title | xml_escape }}",
        "author": "{{ post.author | xml_escape }}",
        "category": "{{ post.category | xml_escape }}",
        "content": {{ post.content | strip_html | strip_newlines | jsonify }},
        "url": "{{ post.url | xml_escape }}"
      }
      {% unless forloop.last %},{% endunless %}
    {% endfor %}
  };
</script>
<script src="{{ site.url }}{{ site.baseurl }}/assets/js/lunr.min.js"></script>
<script src="{{ site.url }}{{ site.baseurl }}/assets/js/search.js"></script>