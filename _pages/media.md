---
layout: archive
title: "Media Coverage"
permalink: /media/
author_profile: true
---


{% if site.talkmap_link == true %}

<p style="text-decoration:underline;"><a href="/talkmap.html">Here is a selection of recent articels and podacasts.</a></p>

{% endif %}

{% for post in site.media reversed %}
  {% include archive-single-talk.html %}
{% endfor %}