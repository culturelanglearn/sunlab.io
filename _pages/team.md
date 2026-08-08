---
title: "Sun Lab - Team"
layout: gridlay
excerpt: "Sun Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We are looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**

Jump to [director](#director), [postdoctoral research fellows](#postdoctoral-research-fellows), [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors).

<a id="director"></a>
## Director
{% assign number_printed = 0 %}
{% for member in site.data.director %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" 
       class="img-responsive" 
       style="width: 150px; height: 150px; object-fit: cover; float: left; margin-right: 15px;" />
  <!-- Add hyperlink to name - with fallback if website doesn't exist -->
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">
        {{ member.name }}
      </a>
    {% else %}
      {{ member.name }}
    {% endif %}
  </h4>
  
  <i>{{ member.info }}</i>
  
  <ul style="overflow: hidden; padding-left: 20px;">

  <!-- Use a loop for education to simplify -->
  {% for i in (1..member.number_educ) %}
    {% assign education_key = 'education' | append: i %}
    {% if member[education_key] %}
      <li>{{ member[education_key] | newline_to_br | markdownify }}</li>
    {% endif %}
  {% endfor %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<a id="postdoctoral-research-fellows"></a>
## Postdoctoral Research Fellows
{% assign number_printed = 0 %}
{% for member in site.data.postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" 
       class="img-responsive" 
       style="width: 150px; height: 150px; object-fit: cover; float: left; margin-right: 15px;" />
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">
        {{ member.name }}
      </a>
    {% else %}
      {{ member.name }}
    {% endif %}
  </h4>
  
  <i>{{ member.info }}</i>
  
  <ul style="overflow: hidden; padding-left: 20px;">

  {% for i in (1..member.number_educ) %}
    {% assign education_key = 'education' | append: i %}
    {% if member[education_key] %}
      <li>{{ member[education_key] | newline_to_br | markdownify }}</li>
    {% endif %}
  {% endfor %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<a id="postdoctoral-research-fellows"></a>
## Incoming PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.phd_students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" 
       class="img-responsive" 
       style="width: 150px; height: 150px; object-fit: cover; float: left; margin-right: 15px;" />
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">
        {{ member.name }}
      </a>
    {% else %}
      {{ member.name }}
    {% endif %}
  </h4>
  
  <i>{{ member.info }}</i>
  
  <ul style="overflow: hidden; padding-left: 20px;">

  {% for i in (1..member.number_educ) %}
    {% assign education_key = 'education' | append: i %}
    {% if member[education_key] %}
      <li>{{ member[education_key] | newline_to_br | markdownify }}</li>
    {% endif %}
  {% endfor %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<a id="staff"></a>
## Staff
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" 
       class="img-responsive" 
       style="width: 150px; height: 150px; object-fit: cover; float: left; margin-right: 15px;" />
  
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">
        {{ member.name }}
      </a>
    {% else %}
      {{ member.name }}
    {% endif %}
  </h4>
  
  <i>{{ member.info }}</i>

  <ul style="overflow: hidden; padding-left: 20px;">

  {% for i in (1..member.number_educ) %}
    {% assign education_key = 'education' | append: i %}
    {% if member[education_key] %}
      <li>{{ member[education_key] | newline_to_br | markdownify }}</li>
    {% endif %}
  {% endfor %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<a id="master-and-bachelor-students"></a>
## Master and Bachelor Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  {% if member.photo %}
    <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" 
         class="img-responsive" 
         style="width: 150px; height: 150px; object-fit: cover; float: left; margin-right: 15px;" />
  {% endif %}
  
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">
        {{ member.name }}
      </a>
    {% else %}
      {{ member.name }}
    {% endif %}
  </h4>
  
  <i>{{ member.info }}</i>
  {% if member.email %}
    <br><a href="mailto:{{ member.email }}">{{ member.email }}</a>
  {% endif %}
  
  <ul style="overflow: hidden; padding-left: 20px;">

  {% for i in (1..member.number_educ) %}
    {% assign education_key = 'education' | append: i %}
    {% if member[education_key] %}
      <li>{{ member[education_key] | newline_to_br | markdownify }}</li>
    {% endif %}
  {% endfor %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<a id="alumni"></a>
## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  {% if member.photo %}
    <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" 
         class="img-responsive" 
         style="width: 150px; height: 150px; object-fit: cover; float: left; margin-right: 15px;" />
  {% endif %}
  
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">
        {{ member.name }}
      </a>
    {% else %}
      {{ member.name }}
    {% endif %}
  </h4>
  
  <i>{{ member.duration }} <br> Role: {{ member.info }}</i>
  {% if member.email %}
    <br><a href="mailto:{{ member.email }}">{{ member.email }}</a>
  {% endif %}
  
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<a id="lab-visitors"></a>
## Former visitors, BSc/ MSc students
<div class="row">

<div class="col-sm-4 clearfix">
<h4>Visitors</h4>
{% for member in site.data.alumni_visitors %}
{{ member.name }}<br>
{% endfor %}
</div>

<div class="col-sm-4 clearfix">
<h4>Master students</h4>
{% for member in site.data.alumni_msc %}
{{ member.name }}<br>
{% endfor %}
</div>

<div class="col-sm-4 clearfix">
<h4>Bachelor Students</h4>
{% for member in site.data.alumni_bsc %}
{{ member.name }}<br>
{% endfor %}
</div>

</div>

<a id="administrative-support"></a>
## Administrative Support
<a href="https://culturelanglearn.github.io/sunlab.io/team/">Audrey Chang</a> and <a href="https://culturelanglearn.github.io/sunlab.io/team/">April Li</a> are helping us (and other groups) with administrative support.
