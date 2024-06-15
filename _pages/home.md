---
title: "TRAILS Lab - Home"
layout: homelay
excerpt: "TRAILS Lab @ University of Illinois Urbana Champaign"
sitemap: false
permalink: /
---

TRAILS LAB website is working!!!!! More details to follow.

Probably replace this with a group image?
<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="4000" data-pause="hover" >
    <div class="carousel-inner" markdown="0">
        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/group.jpg"/>
        </div>
    </div>
</div>


This is taken from Katie's page. Using human-centered computing methods in the context of computer science education, her research improves learners’ motivation and cognition while learning programming, with a long-term goal of broadening pathways to computing education.
Dr. Cunningham’s current focus is on understanding and supporting novice learners with diverse goals, and developing new software-supported scaffolding that allows learners to focus on code’s purpose.

{% for thread in site.data.threads %}

{% if thread.highlight == 1 %}

<div class="row">

<div class="col-sm-12 clearfix">
 <div class="well">
  <pubtit>{{ thread.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ thread.image }}" class="img-responsive" width="33%"/>
  <p>{{ thread.description }}</p>
 </div>
</div>

</div>
{% endif %}
{% endfor %}

<figure class="fourth">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/logo_Illinois.png" style="width: 40px">
</figure>
