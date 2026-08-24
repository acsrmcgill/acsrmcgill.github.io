---
layout: archive
title: "People"
header:
  overlay_image: grouppic.png
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  caption: ""
excerpt: ""
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
<style>
  .people-container {
    display: flex;
    flex-wrap: wrap;
    align-items: flex-start; /* Don't stretch cards to the row's tallest card */
    justify-content: flex-start; /* Align left */
    gap: 15px;
  }
  
  .person-card {
    width: 250px;
    display: flex;
    align-items: flex-start; /* Top-align photo + text so every name lines up */
    gap: 15px; /* Spacing between image and text */
  }
  .person-card img {
    width: 170px;  /* Uniform size */
    height: 170px; /* Uniform size */
    object-fit: cover; /* Prevents stretching/cropping */
    border-radius: 50%; /* Perfectly round */
    border: 2px solid #ddd; /* Optional: subtle border */
    flex-shrink: 0; /* Keep the photo from being squeezed by long bios */
  }
  .person-card figcaption {
    text-align: left; /* Ragged right */
    color: black; /* Ensure black text */
    font-size: 14px;
    width: 100%; /* Ensures proper text wrapping */
    font-family: inherit; /* match site body font instead of theme's serif caption font */
  }
  .person-card b {
    display: block; /* own line, so social icons don't crowd the name */
    font-size: 16px; /* Slightly larger name */
    margin-bottom: 2px;
  }
  /* Social/website icon row under a person's name */
  .person-social {
    display: flex;
    gap: 10px;
    margin: 2px 0 6px;
  }
  .person-social a {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 24px;
    height: 24px;
    border-radius: 4px; /* square (soft corners) instead of round */
    background: #000; /* black badge */
    color: #fff;      /* white icon */
    font-size: 12px;
    text-decoration: none;
  }
  .person-social a:hover {
    background: #555;
  }
  /* Bio links use the site's normal link blue instead of inheriting the card's black text.
     The ">" limits this to links typed directly in the bio text, so it doesn't touch the
     .person-social icon badges above (those are nested one level deeper). */
  .person-card figcaption > a {
    color: #52adc8;
  }
  .person-card figcaption > a:hover {
    color: #3d8298;
  }
  /* Clamp long bios to 3 lines; JS below adds a View more/less toggle only when a bio
     actually overflows, so short placeholder bios don't get a pointless button. */
  .person-bio {
    display: -webkit-box;
    -webkit-line-clamp: 3;
    -webkit-box-orient: vertical;
    overflow: hidden;
  }
  .person-bio.expanded {
    -webkit-line-clamp: unset;
    overflow: visible;
  }
  .person-toggle {
    display: none;
    margin-top: 4px;
    padding: 0;
    background: none;
    border: none;
    color: #52adc8;
    font-size: 13px;
    text-decoration: underline;
    cursor: pointer;
  }
  .person-toggle:hover {
    color: #3d8298;
  }
</style>
# Faculty
{% include feature_row %}
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
      <b>Nikolas Provatas</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">Professor, Canada Research Chair in Computational Materials Science.</span>
    </figcaption>
  </figure>
</div>
# Researchers
{% include feature_row %}
<!-- <img src="{{ base_path }}/images/bio-photo.jpg" alt="Salvador" style="width:10%;height:auto;">
{: style="text-align: justify" }
_**Salvador Valtierra Rodriguez**_. Thermodynamic modeling of stainless steels. Use of calphad driven free energies to parameterize phase field equations and simulate phase transformations in stainless steels.
 [[more]](../_pages/404.md) -->
  
<div class="people-container">
  <figure class="person-card">
    <img src="{{ base_path }}/images/profile_pics/daniel.jpg" alt="Daniel Coelho">
    <figcaption>
      <b>Daniel Coelho</b>
      <span class="person-social">
        <a href="https://dancoelho.github.io" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="https://github.com/dancoelho" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="https://www.linkedin.com/in/coelhodl/" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">Postdoctoral Fellow. My research interests lie at the intersection of condensed matter physics and materials science and engineering.</span>
    </figcaption>
  </figure>
  <figure class="person-card">
    <img src="{{ base_path }}/images/bio-photo.jpg" alt="Mingwang Zhong">
    <figcaption>
      <b>Mingwang Zhong</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">Postdoctoral Fellow. Description.</span>
    </figcaption>
  </figure>
  <figure class="person-card">
    <img src="{{ base_path }}/images/profile_pics/ravneet.png" alt="Ravneet Kaur">
    <figcaption>
      <b>Ravneet Kaur</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="https://www.linkedin.com/in/ravneet-kaur-bains/" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">Research Assistant. My research applies the Structural Phase Field Crystal (XPFC) formalism to study the microstructure formation in additively manufactured alloys. I examine how dislocations mediate the nucleation of Si precipitates in Al-Si alloys during Laser Powder Bed Fusion (LPBF), through large-scale three-dimensional simulations that resolve atomic-scale defects while evolving on diffusive timescales. This work is built on OpenPFC, an open-source C++/MPI framework that I have extended from pure materials to binary alloys.</span>
    </figcaption>
  </figure>
</div>
# Graduate students
{% include feature_row %}
<div class="people-container">
  <figure class="person-card">
    <img src="{{ base_path }}/images/profile_pics/tristan.png" alt="Tristan Devaux">
    <figcaption>
      <b>Tristan Devaux</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">PhD student. Co-supervised with <a href="https://www.physics.mcgill.ca/~cumming/" target="_blank">Prof. Andrew Cumming</a>. My research focuses on the properties and states of matter at high density inside of compact stars. I am working on creating statistical field theory - based on Phase-Field Crystal (PFC) -  of the so-called “nuclear pasta” phases, which are expected to emerge at subnuclear densities in the crust of neutron stars.</span>
    </figcaption>
  </figure>
  <figure class="person-card">
    <img src="{{ base_path }}/images/bio-photo.jpg" alt="Sammohith Nittala">
    <figcaption>
      <b>Sammohith Nittala</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">PhD student. Description.</span>
    </figcaption>
  </figure>
  <figure class="person-card">
    <img src="{{ base_path }}/images/bio-photo.jpg" alt="Tomoji">
    <figcaption>
      <b>Tomoji</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">Masters student. Description.</span>
    </figcaption>
  </figure>
  <figure class="person-card">
    <img src="{{ base_path }}/images/profile_pics/justin.png" alt="Justin Mainville">
    <figcaption>
      <b>Justin Mainville</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">Masters student. <a href="https://www.bioelectrochemistry.mcgill.ca/justin-mainville.html" target="_blank">Quantitative phase field modelling of stress-corrosion-cracking</a>. In recent years, the phase field method has proven itself to be a powerful and versatile method to model solidification and fractures. However, it is far from being limited to those fields and recent studies has shown that phase field is ideal to study corrosion. Utilizing recent phase field models of stress-corrosion-cracking, I will create a workflow to parameterize those models to experiments. Thus, making them suitable to reproduce experimental work, and offering an in-silico way to quantitatively study the process of stress-corrosion-cracking in various materials.</span>
    </figcaption>
  </figure>
</div>
<!-- <img src="{{ base_path }}/images/profile_pics/daniel.jpg" alt="Daniel" style="width:10%;height:auto;">
{: style="text-align: justify" }
_**Daniel Coelho**_. PhD student. My research interests lie at the intersection of condensed matter physics and materials science and engineering.
 [[more]](../_pages/404.md) -->
<!-- <br><br> -->
<!-- {% include feature_row id="grads" type="left" %} -->
# Undergradute students
{% include feature_row %}
# Alumni and past members
{% include feature_row %}  
<div class="people-container">
  <figure class="person-card">
    <img src="{{ base_path }}/images/bio-photo.jpg" alt="Jaarli Suviranta">
    <figcaption>
      <b>Jaarli Suviranta</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">I'm a PhD student in his last year completing my work on solidification studies using PFC.</span>
    </figcaption>
  </figure>
  <figure class="person-card">
    <img src="{{ base_path }}/images/bio-photo.jpg" alt="Duncan Burns">
    <figcaption>
      <b>Duncan Burns</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">A longtime swimmer and culinary enthusiast, mmm pool noodles...</span>
    </figcaption>
  </figure>
  <figure class="person-card">
    <img src="{{ base_path }}/images/profile_pics/paul.png" alt="Paul Jreidini">
    <figcaption>
      <b>Paul Jreidini</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">Developed Phase Field Crystal (PFC) models and their amplitude expansions for a variety of use cases, including: • Studying nucleation rates at the scale boundary between traditional atomic and mesoscale models • Reproducing experimentally observed orientation gradients in rapidly solidifying aluminum samples using three-phase (solid, liquid, gas) Amplitude PFC models with quantitative pure-material phase diagrams • Examining cavitation in droplets of materials that undergo anomalous expansion during solidification (e.g. water and silicon) and comparing to published experiments • Proof-of-concept work on the application of PFC methodology on various long-term topics such as martensitic transformations, multi-component amorphous materials, neutron star crust material</span>
    </figcaption>
  </figure>
     <figure class="person-card">
      <img src="{{ base_path }}/images/bio-photo.jpg" alt="Salvador Valtierra Rodriguez">
      <figcaption>
        <b>Salvador Valtierra Rodriguez</b>
        <span class="person-social">
          <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
          <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
          <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
        </span>
        <span class="person-bio">Postdoctoral researcher. Thermodynamic modeling of stainless steels.</span>
      </figcaption>
    </figure>
  <figure class="person-card">
    <img src="{{ base_path }}/images/profile_pics/jonathan.png" alt="Jonathan Stolle">
    <figcaption>
      <b>Jonathan Stolle</b>
      <span class="person-social">
        <a href="#" target="_blank" title="Website"><i class="fa fa-globe" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="GitHub"><i class="fab fa-github" aria-hidden="true"></i></a>
        <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i></a>
      </span>
      <span class="person-bio">General physics enthusiast with a focus on non-linear systems: B.Eng. Engineering Physics McMaster 2006, M.Sc. Physics (Atmospheric Physics) McGill 2009, Postdoctoral Fellow at North Eastern University 2013-2014 (Ca2+ transport in heart cells). 11 years experience in telematics in industry as a(n application) software developer and data analyst (mainly time-series analysis). Visits the (Montreal and Hamilton) ACSR from time-to-time.</span>
    </figcaption>
  </figure>
</div>

<script>
document.addEventListener('DOMContentLoaded', function () {
  document.querySelectorAll('.person-bio').forEach(function (bio) {
    // Only add a toggle if the bio is actually being clamped/truncated
    if (bio.scrollHeight > bio.clientHeight + 1) {
      var btn = document.createElement('button');
      btn.type = 'button';
      btn.className = 'person-toggle';
      btn.textContent = '[More]';
      btn.style.display = 'inline-block';
      btn.addEventListener('click', function () {
        var expanded = bio.classList.toggle('expanded');
        btn.textContent = expanded ? '[Less]' : '[More]';
      });
      bio.insertAdjacentElement('afterend', btn);
    }
  });
});
</script>