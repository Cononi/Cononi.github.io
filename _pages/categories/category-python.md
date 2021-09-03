---
title: "Python 프록래밍"
layout: archive
permalink: /categories/Python/
author_profile: true
sidebar_main: true
---
{% assign posts = site.categories.Python %}
{% if site.data.categories contains page.permalink %}
    {% for post in posts %} 
        {% include archive-single.html type=page.entries_layout %} 
    {% endfor %}
{% endif %}