---
layout: archive
title: "People"
permalink: /people/
author_profile: true
redirect_from: 
  - /acsr/
  - /acsr.html
grads:
  - image_path: image-alignment-150x150.jpg
    title: "Left aligned placeholder 1"
    excerpt: "Left-aligned image centered with"
    url: ""
    btn_label: "Read More"
    btn_class: "btn--primary"
---
{% include feature_row %}


## Faculty

{% include group-by-array collection=site.posts field="categories" %}

<!-- <div class="cf"> 
<div class="grid__wrapper">

{% for category in group_names %} -->
  <!-- only research -->
<!--   {% if category contains site.research %}
    {% assign posts = group_items[forloop.index0] %}
    {% for post in posts %}
    {% include archive-single.html type="grid" %}
    {% endfor %}
  {% endif %}
{% endfor %}

</div>
</div> -->


## Post-doctoral researchers and visitors

## Graduate students

<!-- {% include feature_row id="grads" type="left" %} -->


## Undergradute students

## Alumni and past members
