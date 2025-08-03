---
title: "WOWinfo" # 사이드바 카테고리 눌렀을 때 본문부분에 나오는 문구
layout: archive
permalink: /wowinfo
author_profile: true
sidebar:
    nav: "sidebar-category"
---


{% assign posts = site.categories.wowinfo %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}