---
layout: page
permalink: /publications/
title: publications
description: Also see <a href="https://scholar.google.com/citations?user=3uTVQt0AAAAJ">Google Scholar</a> and <a href="https://www.semanticscholar.org/author/Swabha-Swayamdipta/2705113">Semantic Scholar</a>
years: [2021, 2020, 2019, 2018, 2017, 2016, 2014, 2012]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
