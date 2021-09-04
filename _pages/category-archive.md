---
title: "Posts by Category"
permalink: /categories/
author_profile: true
#sidebar:
#  title: "Sample Title"
#  nav: sidebar-profile
---
<ul class="taxonomy__index">
    {% for category in site.categories %}
       {% if site.data.categories contains category[0] %}
        <li>
          <a href="{{category[0]}}">
            <strong>{{ category[0] }}</strong> <span class="taxonomy__count">{{ category[1].size }}</span>
          </a>
        </li>
      {% endif %}
    {% endfor %}
</ul>