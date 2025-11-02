---
layout: default
title: "PI (Professor)"
permalink: /team/pi/
---

# 🎓 Principal Investigator (PI)

{% assign pis = site.members | where: "role", "pi" %}

{% for person in pis %}
    {% render person with person %}
{% endfor %}
