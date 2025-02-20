---
title: "TRAILS Lab - Publications"
layout: gridlay
excerpt: "TRAILS Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Group highlights

**At the end of this page, you can find the [full list of publications](#full-list-of-publications).

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
  <nobr>
  {% for link in publi.logos %}
   <span></span><span class="publication-logo"><a href="{{link.link }}">{{ link.name }}</a></span>
  {% endfor %}
 </nobr>
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


## Full List of Publications

{% for publi in site.data.publist %}

  {{ publi.authors }}. {{publi.year}}. <b>{{ publi.title }}</b>.
  <em><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></em>. {% if publi.note %}{{ publi.note }}{% endif %}

{% endfor %}
