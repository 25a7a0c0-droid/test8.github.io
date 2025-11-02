---
layout: single
title: "PI (Professor)"
permalink: /team/pi/
---

# 🎓 Principal Investigator (PI)

{% assign pis = site.members | where: "role", "pi" %}

{% for person in pis %}
<div class="profile-card">
    <h2>{{ person.name }}</h2> 
    <p>{{ person.title }}</p> 
    {{ person.content | markdownify }} 
</div>
{% endfor %}
