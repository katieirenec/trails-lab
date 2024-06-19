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


We want all computing learners to achieve their goals (and perhaps aim for goals they previously thought impossible). We respect that different learners want to reach different endpoints with their computing knowledge, and meeting the needs of all learners will require building a variety of pathways to computing education.

We believe that everyone should have the opportunity to learn computing in a way that motivates them and supports their needs. We use approaches from human-computer interaction and computing education to understand learners' goals and experiences, build educational interventions inspired by learning theory, and evaluate the effectiveness of these new approaches. 

Our name is inspired by the efforts of the National Park Service to make breathtakingly beautiful and previously inaccessible wilderness reachable by the general public. 

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
