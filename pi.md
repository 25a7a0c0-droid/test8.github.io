---
layout: default 
title: "PI (Professor)"
permalink: /team/pi/
---

# 🎓 Principal Investigator (PI)

{% assign pis = site.members | where: "role", "pi" %}

{% for person in pis %}

<section>
    <h2>{{ person.name }}</h2> 
    <p>{{ person.affiliation }} | {{ person.role }}</p>
    
    {% if person.image %}
        <img src="{{ person.image | relative_url }}" alt="{{ person.name }} photo">
    {% endif %}

    <div class="bio">
        {{ person.content | markdownify }} 
    </div>
</section>
{% endfor %}
