---
layout: archive
title: "Media Coverage"
permalink: /media/
author_profile: true
---

{% include base_path %}

Here is a selection of recent articels and podacasts ... soon =)  
Find further up-to-date resources at <a href="https://linktr.ee/sciphie">linktr.ee/sciphie </a>

{% for post in site.media reversed %}
  {% include archive-single-media.html %}
{% endfor %}

