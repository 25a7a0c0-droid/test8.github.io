---
layout: default
title: "Research Members"
permalink: /team/member/
---

# 🧑‍💻 Research Members

{% assign members = site.members | where_exp: "person", "person.role != 'pi'" %}

{% for person in members %}
<section>
    <h3>{{ person.name }} ({{ person.role }})</h3> 
    <p>{{ person.affiliation }}</p>
    
    <div class="bio">
        {{ person.content | markdownify }} 
    </div>
</section>
{% endfor %}
