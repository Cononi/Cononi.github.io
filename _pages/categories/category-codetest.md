---
title: "코드 테스트"
layout: archive
permalink: /categories/Codetest/
author_profile: true
sidebar_main: true
---
{% assign posts = site.categories.Codetest %}
{% if site.data.categories contains page.permalink %}
    {% for post in posts %} 
        {% include archive-single.html type=page.entries_layout %} 
    {% endfor %}
{% endif %}

