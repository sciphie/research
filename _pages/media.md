---
layout: archive
title: "Media Coverage"
permalink: /media/
author_profile: true
---

{% include base_path %}

Here is a selection of recent articels and podacasts ... soon =)  
Find further up-to-date resources at <li><a href="https://linktr.ee/sciphie"><i class="fas fa-fw fa-key" aria-hidden="true"></i> linktr.ee/sciphie </a></li> 

{% for post in site.media reversed %}
  {% include archive-single-media.html %}
{% endfor %}

