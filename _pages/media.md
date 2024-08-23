---
title: "Khwarizmi Lab - Media Coverage"
layout: textlay
excerpt: "Media Coverage @ Khwarizmi Lab"
sitemap: true
permalink: /media.html
---

# Media Coverage

{% for article in site.data.media %}
<h4>{{ article.date }}</h4>
<p style="font-size: larger !important;"><em>{{ article.headline }}</em></p>
{% endfor %}
