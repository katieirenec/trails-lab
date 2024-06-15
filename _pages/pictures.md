---
title: "TRAILS Lab - Pictures"
layout: piclay
excerpt: "TRAILS Lab -- Pictures"
permalink: /pictures/
---

# Pictures

## ICER 2024

{% assign number_printed = 0 %}
{% if site.data.pictures_icer2024.size == 0 %}
To be updated.
{% endif %}

{% for pic in site.data.pictures_icer2024 %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
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
