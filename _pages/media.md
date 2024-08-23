---
title: "Khwarizmi Lab - Media Coverage"
layout: textlay
excerpt: "Media Coverage @ Khwarizmi Lab"
sitemap: true
permalink: /media.html
---

# Media Coverage

{% for article in site.data.media %}
<h3>{{ article.date }}</h3>
<h4><em>{{ article.headline }}</em></h4>
{% endfor %}
