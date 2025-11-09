---
title: "News"
layout: textlay
excerpt: "Culture, Language, & Learning Lab at Hong Kong Polytechnic University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br> {{ article.headline | markdownify}}</p>
{% endfor %}
