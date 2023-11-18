---
title: "Khwarizmi Lab - Pictures"
layout: piclay
excerpt: "Khwarizmi Lab -- Pictures"
sitemap: true
permalink: /pictures/
---

# Pictures


#### Gallery
(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.gallery %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
<p style="margin-left:10px !important;">
<strong>{{ pic.title }}</strong><br/>
<em>{{ pic.date }}</em>
</p>
<img src="{{ site.url }}{{ site.baseurl }}/images/gallery/{{ pic.image }}" alt="{{ pic.alt }}" class="img-responsive" width="100%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>
