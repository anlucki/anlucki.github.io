---
layout: splash
permalink: /
hidden: true
title: "Welcome!"
header:
  overlay_color: "#434C5E"
excerpt: >
  Hey, welcome to my blog!<br />
  <small>Not much to see around (<em>yet</em> 🤪). Feel free to explore around, more content incoming!</small>
pagination:
  enabled: true
---

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% for post in paginator.posts %}
  {% include archive-single.html %}
{% endfor %}

{% include paginator.html %}