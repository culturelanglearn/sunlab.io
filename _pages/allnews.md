---
title: "News"
layout: textlay
excerpt: "Culture, Language, & Learning Lab at Hong Kong Polytechnic University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<b>{{ article.date }}</b> <br> {{ article.headline }}
{% endfor %}

<!-- Audrey commented out to remove the <p> marking 09/11/2025
{% for article in site.data.news %}
{{ article.date }} <br> {{ article.headline | markdownify}}
{% endfor %}
--> 
