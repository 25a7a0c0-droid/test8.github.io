---
title: Projects
nav:
  order: 2
  tooltip: Mental health, AI and more
---

# {% include icon.html icon="fa-solid fa-wrench" %}Projects

Our current projects

{% include tags.html tags="publication, resource, website" %}

{% include search-info.html %}

{% include section.html %}

## Featured

{% include list.html component="card" data="projects" filter="group == 'featured'" %}

{% include section.html %}

## More

{% include list.html component="card" data="projects" filter="!group" style="small" %}
