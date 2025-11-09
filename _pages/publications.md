---
title: "Sun Lab - Publications"
layout: gridlay
excerpt: "Sun Lab -- Publications."
sitemap: false
permalink: /publications
---
## Google Scholar 
Check out Dr. Sun's [google scholar](https://scholar.google.com/citations?user=Deh6LRUAAAAJ&hl=en) for a full list of publications and links. 

## Full List of publications

{% for publi in site.data.publist %}
  {{ publi.authors }} ({{ publi.year }}). {{ publi.title }}. <em>{{ publi.journal }}</em>, <em>{{ publi.volume }}</em>{% if publi.issue %}({{ publi.issue }}){% endif %}{% if publi.pages %}, {{ publi.pages }}{% endif %}. {% if publi.doi %}https://doi.org/{{ publi.doi }}{% else %}<a href="{{ publi.link.url }}">{{ publi.link.display }}</a>{% endif %}
  <br /><br />
{% endfor %}

<!-- original format - AUDREY COMMENTED OUT 09/11/2025 
# Publications

## Group highlights

**At the end of this page, you can find the [full list of publications and patents](#full-list-of-publications). All papers are also available on [arXiv](https://arxiv.org/search/?searchtype=author&query=Allan%2C+M+P).**

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Full List of publications

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
-->
