---
title: "Khwarizmi Lab - Media Coverage"
layout: textlay
excerpt: "Media Coverage @ Khwarizmi Lab"
sitemap: true
permalink: /media.html
---

# Media Coverage

{% for article in site.data.media %}
<p><b style="font-size: 21px !important;">{{ article.date }}</b>: <em style="font-size: 22px !important;">{{ article.headline }}</em></p>
{% endfor %}
