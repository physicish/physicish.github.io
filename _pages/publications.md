---
layout: page
title: publications
nav: true
nav_order: 1
dropdown: true
children: 
    - title: preprints
      permalink: /publications/preprints
    - title: articles
      permalink: /publications/articles
    - title: theses
      permalink: /publications/theses
---
<!-- _pages/publications.md -->
<div class="publications">

  Up-to-date list of publications available on <a href="https://scholar.google.com/citations?user=Ufpa6SIAAAAJ">Google Scholar</a>, <a href="https://www.researchgate.net/profile/Matteo-Barbetti">ResearchGate</a> or <a href="https://inspirehep.net/authors/1908127">Inspire HEP</a>.

  <h2 class="pub-type">preprints</h2>
  {%- for y in page.preprints-years -%}
    <h2 class="year">{{y}}</h2>
    {%- bibliography -f preprints -q @*[year={{y}}]* -%}
  {%- endfor -%}

  <h2 class="pub-type">conference & journal articles</h2>
  {%- for y in page.articles-years -%}
    <h2 class="year">{{y}}</h2>
    {%- bibliography -f articles -q @*[year={{y}}]* -%}
  {%- endfor -%}

  <h2 class="pub-type">theses</h2>
  {%- for y in page.theses-years -%}
    <h2 class="year">{{y}}</h2>
    {%- bibliography -f theses -q @*[year={{y}}]* -%}
  {% endfor %}

</div>
