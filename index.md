---
---

# Testlab's website

Welcome to our Test lab. welcome welcome

{% include section.html %}

## Highlights

{% capture text %}

Click to see our prevent research.

{%
  include button.html
  link="research"
  text="See our publications"
  icon="fa-solid fa-arrow-left"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="research"
  title="Our Research"
  text=text
%}

{% capture text %}

Click to see our recent news.

{%
  include button.html
  link="news"
  text="Browse our news"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="news"
  title="Recent news"
  flip=true
  style="bare"
  text=text
%}

