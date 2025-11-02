---
layout: default
title: "PI (Professor)"
permalink: /team/pi/
---

# 🎓 Principal Investigator (PI)

{% assign pis = site.members | where: "role", "pi" %}

{% for person in pis %}
<section class="member-profile">
    {# Front Matter의 'name'을 H2로 출력 #}
    <h2>{{ person.name }}</h2> 
    {# Front Matter의 다른 정보들을 출력 #}
    <p>{{ person.affiliation }} | {{ person.role }}</p>
    
    {% if person.image %}
        <img src="{{ person.image | relative_url }}" alt="{{ person.name }} photo">
    {% endif %}

    <div class="bio">
        {# Markdown 본문 내용 ('Professor of yonsei university' 등)을 HTML로 변환하여 출력 #}
        {{ person.content | markdownify }} 
    </div>
</section>
{% endfor %}
