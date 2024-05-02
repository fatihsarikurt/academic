---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

{% for post in site.talks reversed %}
  {% include archive-single-talk.html %}
{% endfor %}


{% if site.author.googlescholar %}
  <div class="wordwrap">Please refer to <a href="{{site.author.googlescholar}}">for a full list of my publications.</a>.</div>
{% endif %}