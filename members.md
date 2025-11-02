---
layout: single
title: "Research Members"
permalink: /team/member/
---

# 🧑‍💻 Research Members

{% assign members = site.members | where_exp: "person", "person.role != 'pi'" %}

{% for person in members %}
<div class="member-card">
    <h3>{{ person.name }} ({{ person.role }})</h3> 
    
    {{ person.content | markdownify }} 
</div>
{% endfor %}
