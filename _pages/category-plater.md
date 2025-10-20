---
title: "Plater" # 사이드바에서 카테고리 눌렀을 때 본문부분에 나오는 문구
layout: archive
permalink: /plater
author_profile: true
sidebar:
    nav: "sidebar-category"
---


{% assign posts = site.categories.Plater %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}