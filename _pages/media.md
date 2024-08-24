---
title: "Khwarizmi Lab - Media Coverage"
layout: textlay
excerpt: "Media Coverage @ Khwarizmi Lab"
sitemap: true
permalink: /media.html
---

# Media Coverage

{% for article in site.data.media %}
<p><b style="font-size: 24px !important;">{{ article.date }}</b>: <em>{{ article.headline }}</em></p>
{% endfor %}
