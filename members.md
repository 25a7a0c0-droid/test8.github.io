---
layout: default
title: "Research Members"
permalink: /team/member/
---

# 🧑‍💻 Research Members

{% assign members = site.members | where_exp: "person", "person.role != 'pi'" %}

{% for person in members %}
<section class="member-profile">
    {# Front Matter의 'name'을 H3로 출력하고, role 정보를 괄호 안에 추가 #}
    <h3>{{ person.name }} ({{ person.role }})</h3> 
    <p>{{ person.affiliation }}</p>
    
    {% if person.image %}
        <img src="{{ person.image | relative_url }}" alt="{{ person.name }} photo">
    {% endif %}
    
    <div class="bio">
        {# Markdown 본문 내용을 HTML로 변환하여 출력 #}
        {{ person.content | markdownify }} 
    </div>
</section>
{% endfor %}
