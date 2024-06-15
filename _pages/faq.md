---
title: "faq"
layout: textlay
excerpt: "TRAILS Lab @ University of Illinois Urbana-Champaign"
sitemap: true
permalink: /faq.html
---

# Frequently Asked Questions

{% for article in site.data.faq %}
<div class="faq-item"><p class="faq-question">**{{ article.q }}**</p> <br> {{ article.a}}
{% endfor %}
