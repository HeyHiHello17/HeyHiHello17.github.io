---
layout: default
title: "Blog"
description: 아주 가끔씩 관심 분야의 글을 올려요.
main: true
project-header: true
header-img: img/about.jpg
---

<div class="catalogue" style="max-width:750px;margin:0 auto;">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.blog == true %}
{% include post-list.html %}
{% endif %}
{% endfor %}
</ul>
