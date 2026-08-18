---
title: "Discussion Papers"
permalink: /discussion-papers/
layout: single
author_profile: true
sidebar:
  nav: "sidebar"
---

{% assign papers = site.discussion_papers | sort: "date" | reverse %}
{% if papers.size > 0 %}
<ul>
  {% for paper in papers %}
  <li><a href="{{ paper.url | relative_url }}">{{ paper.title }}</a></li>
  {% endfor %}
</ul>
{% else %}
아직 올라온 발제문이 없습니다.
{% endif %}
