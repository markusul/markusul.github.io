---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---


  You can also find my articles on <a href="https://scholar.google.com/citations?user=P7zvodEAAAAJ&hl=en">my Google Scholar profile</a>.


{% include base_path %}

{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
<h1>{{ category[1].title }}</h1><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

