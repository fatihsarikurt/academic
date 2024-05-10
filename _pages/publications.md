---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

## Journal Publications

{% for post in site.publications reversed %}
  {% if post.type == 'publications' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Conference Publications

{% for post in site.publications reversed %}
  {% if post.type == 'conference' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}


{% if site.author.googlescholar %}
  <div class="wordwrap">Please refer to <a href="{{site.author.googlescholar}}">Google Scholar</a> for a full list of my publications.</div>
{% endif %}