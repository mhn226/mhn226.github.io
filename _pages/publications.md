---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}


### 2020

{% for post in site.publications %}
  {% capture year %}{{post.date | date: "%Y"}}{% endcapture %}
  {% if year == '2020' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}


### 2019

{% for post in site.publications %}
  {% capture year %}{{post.date | date: "%Y"}}{% endcapture %}
  {% if year == '2019' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
