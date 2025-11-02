---
layout: single
title: "PI (Professor)"
permalink: /team/pi/
---

# 🎓 Principal Investigator (PI)

{% comment %}
  _members 컬렉션에서 role이 'pi'인 항목만 필터링하여 불러옵니다.
{% endcomment %}
{% assign pis = site.members | where: "role", "pi" %}

{% for person in pis %}
<div class="pi-profile">
    <h2>{{ person.name }}</h2> 
    <p>{{ person.title }}</p> 
    
    {# 멤버 파일의 본문 내용(소개글)을 여기에 표시합니다. #}
    {{ person.content | markdownify }} 
</div>
{% endfor %}
