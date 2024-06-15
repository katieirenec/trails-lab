---
title: "News"
layout: textlay
excerpt: "TRAILS Lab @ University of Illinois Urbana-Champaign"
sitemap: false
permalink: /news.html
---

# News

{% for article in site.data.news %}
<p>**{{ article.date }}** <br> {{ article.headline }}</p>
{% endfor %}
