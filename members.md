---
layout: default
title: "Research Members"
permalink: /team/member/
---

# 🧑‍💻 Research Members

{% assign members = site.members | where_exp: "person", "person.role != 'pi'" %}

{% for person in members %}
    {% render person with person %}
{% endfor %}
