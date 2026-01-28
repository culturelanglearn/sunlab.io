---
title: "Sun Lab - Publications"
layout: gridlay
excerpt: "Sun Lab -- Publications."
sitemap: false
permalink: /publications
---
## Google Scholar 
Check out Dr. Sun's [google scholar](https://scholar.google.com/citations?user=Deh6LRUAAAAJ&hl=en) for a full list of publications and links. 

## Full List of Journal Publications

{% for publi in site.data.publist %}
  <strong>{{ forloop.index }}.</strong> 
  {{ publi.authors | replace: "Sun, X.", "<b>Sun, X.</b>" }} ({{ publi.year }}). {{ publi.title }}. <em>{{ publi.journal }}</em>, <em>{{ publi.volume }}</em>{% if publi.issue %}({{ publi.issue }}){% endif %}{% if publi.pages %}, {{ publi.pages }}{% endif %}. {% if publi.doi %}<a href="https://doi.org/{{ publi.doi }}">https://doi.org/{{ publi.doi }}</a>{% else %}<a href="{{ publi.link.url }}">{{ publi.link.display }}</a>{% endif %}{% if publi.featured %}<br><b>{{ publi.featured }}</b>{% endif %}
  <br />
{% endfor %}

## Full List of Book Chapters 
Huo, M., Sun, X., Kovelman, I., & Chen, B. (2023). Literacy development in Southeast Asia. In Verhoeven (Ed.), Variation in Literacy Development. Cambridge, UK: Cambridge University Press https://doi.org/10.1017/9781009242585

Michal, A., Fansher, M., Sun, X., Zhang, H., & Shah, P. (2018). Cognitive development. The Oxford Handbook of Educational Psychology. Oxford, UK: Oxford University Press https://doi.org/10.1093/oxfordhb/9780199841332.013.7
<img width="468" height="128" alt="image" src="https://github.com/user-attachments/assets/8595393e-2e69-49f5-be26-559aa4272d48" />


## Public outreach & Non-academic Publications
Q&A with Dr. Xin Sun on exploring infant & toddler minds (lexico-semantic representations) (June 11, 2025). UBC Language Sciences. Link to the interview: https://languagesciences.ubc.ca/news/june-06-2025/qa-dr-xin-sun-exploring-infant-toddler-minds-lexico-semantic-representations

Invited Community Talk: The Bilingual Child (May 21, 2024). United Chinese Community Enrichment Services Society (S.U.C.C.E.S.S), Coquitlam, Canada

Tea for Teaching Podcast: Beware the myth: learning styles affect parents’, children’s, and teachers’ thinking about children’s academic potential. Link to the episode: https://www.podbean.com/media/share/pb-imzr4-14fbbd4

Impacts of the COVID-19 disruption on the language and literacy development of monolingual and heritage bilingual children in the United States: Q&A with Xin Sun. (December 5, 2022). UBC Language Sciences. Link to the interview: https://languagesciences.ubc.ca/news-events/announcement-research-news/dec-5-2022-impacts-covid-19-disruption-language-and-literacy

Graduate Research Spotlight - Xin Sun (2022). Link to the interview: https://lsa.umich.edu/psych/news-events/all-news/graduate-news/graduate-research-spotlight---xin-sun.html 

Sun, X., Nancekivell, S., Gelman, S., & Shah, P. (2021). How mindset beliefs mean differently to Chinese and US students. npj Science of Learning Community Behind the Paper Blog Post 

Sun, X. (2021). Debunking the myth of learning styles: A case for evidence-based instruction and communication. Intercom
(Magazine of the Society for Technical Communication). 68(5), 31-33. 

Sun, X. (2010). Dream [in Chinese]. Journal of Poetry (诗刊). 24, 77. 
<img width="468" height="455" alt="image" src="https://github.com/user-attachments/assets/d6bd03c9-c86d-4a18-85da-3f450851a67f" />


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
