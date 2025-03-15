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

<style>
  .people-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start; /* Align left */
    gap: 20px;
  }
  
  .person-card {
    width: 250px;
    display: flex;
    align-items: center;
    gap: 15px; /* Spacing between image and text */
  }

  .person-card img {
    width: 120px;  /* Uniform size */
    height: 120px; /* Uniform size */
    object-fit: cover; /* Prevents stretching/cropping */
    border-radius: 50%; /* Perfectly round */
    border: 2px solid #ddd; /* Optional: subtle border */
  }

  .person-card figcaption {
    text-align: left; /* Ragged right */
    color: black; /* Ensure black text */
    font-size: 14px;
    width: 100%; /* Ensures proper text wrapping */
  }

  .person-card b {
    font-size: 16px; /* Slightly larger name */
  }
</style>



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

<div class="people-container">
  <figure class="person-card">
    <img src="{{ base_path }}/images/profile_pics/nik.jpg" alt="Nikolas Provatas">
    <figcaption>
      <b>Nikolas Provatas</b><br>
      Professor, Canada Research Chair in Computational Materials Science.
    </figcaption>
  </figure>

</div>


## Researchers

<!-- <img src="{{ base_path }}/images/bio-photo.jpg" alt="Salvador" style="width:10%;height:auto;">
{: style="text-align: justify" }
_**Salvador Valtierra Rodriguez**_. Thermodynamic modeling of stainless steels. Use of calphad driven free energies to parameterize phase field equations and simulate phase transformations in stainless steels.
 [[more]](../_pages/404.md) -->

<div class="people-container">
   <figure class="person-card">
    <img src="{{ base_path }}/images/bio-photo.jpg" alt="Salvador Valtierra Rodriguez">
    <figcaption>
      <b>Salvador Valtierra Rodriguez</b><br>
      Postdoctoral researcher. Thermodynamic modeling of stainless steels.
    </figcaption>
  </figure>
</div>


## Graduate students

<div class="people-container">

  <figure class="person-card">
    <img src="{{ base_path }}/images/bio-photo.jpg" alt="Jaarli Suviranta">
    <figcaption>
      <b>Jaarli Suviranta</b><br>
      I'm a PhD student in his last year completing my work on solidification studies using PFC. 
    </figcaption>
  </figure>

  <figure class="person-card">
    <img src="{{ base_path }}/images/profile_pics/daniel.jpg" alt="Daniel Coelho">
    <figcaption>
      <b>Daniel Coelho</b><br>
      PhD student. My research interests lie at the intersection of condensed matter physics and materials science and engineering.
    </figcaption>
  </figure>

  <figure class="person-card">
    <img src="{{ base_path }}/images/profile_pics/ravneet.jpg" alt="Daniel Coelho">
    <figcaption>
      <b>Ravneet Kaur</b><br>
      Masters student. Currently working on my research project focused on the Structural Phase Field Crystal (XPFC) Vapor Model for binary alloys.
    </figcaption>
  </figure>



</div>


<!-- <img src="{{ base_path }}/images/profile_pics/daniel.jpg" alt="Daniel" style="width:10%;height:auto;">
{: style="text-align: justify" }
_**Daniel Coelho**_. PhD student. My research interests lie at the intersection of condensed matter physics and materials science and engineering.
 [[more]](../_pages/404.md) -->

<!-- <br><br> -->


<!-- {% include feature_row id="grads" type="left" %} -->


## Undergradute students

<figure>
  <left>
    <img src="{{ base_path }}/images/bio-photo.jpg" style="width: 150px;height: 150px;object-fit: contain;">
    <figcaption style="text-align: left;width:30%">
      <b>Justin Mainville</b>.
    </figcaption>
  </left>
</figure>


## Alumni and past members
<figure>
  <left>
    <img src="{{ base_path }}/images/bio-photo.jpg" style="width: 150px;height: 150px;object-fit: contain;">
    <figcaption style="text-align: left;width:30%">
      <b>Duncan Burns</b>. A longtime swimmer and culinary enthusiast, mmm pool noodles... 
    </figcaption>
  </left>
</figure>