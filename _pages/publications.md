---
layout: page
permalink: /publications/
title: publications
description: <sup>*</sup> equal contribution &nbsp;·&nbsp; <sup>†</sup> co-corresponding author &nbsp;·&nbsp; <u>underlined</u> names are students I supervise
nav: true
nav_order: 2
---

<style>
  /* my own name: bold, and drop al-folio's default underline */
  .publications .author > em { border-bottom: none !important; font-style: normal; font-weight: 700; }
  /* supervised students: solid underline rather than the default dashed link style */
  .publications .author a { border-bottom: 1px solid !important; text-decoration: none; }
  .bibliography-category { margin-top: 2.5rem; }
</style>

{% include bib_search.liquid %}

<div class="publications">

<h2 class="bibliography-category">Preprints</h2>

{% bibliography --query @*[preprint=true]* %}

<h2 class="bibliography-category">Peer-Reviewed Publications</h2>

{% bibliography --query @*[peerreviewed=true]* %}

</div>
