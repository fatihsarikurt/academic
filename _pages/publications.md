---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<h2>Journal Publications</h2>
<ul>
  {% for post in site.publications reversed %}
    {% if post.path contains '_publications/journal' %}
      <li>
        {% include archive-single.html %}
      </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Conference Publications</h2>
<ul>
  {% for post in site.publications reversed %}
    {% if post.path contains '_publications/conference' %}
      <li>
        {% include archive-single.html %}
      </li>
    {% endif %}
  {% endfor %}
</ul>


{% if site.author.googlescholar %}
  <div class="wordwrap">Please refer to <a href="{{site.author.googlescholar}}">Google Scholar</a> for a full list of my publications.</div>
{% endif %}