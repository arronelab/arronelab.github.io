---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<script
  src="https://code.jquery.com/jquery-3.4.1.min.js"
  integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo="
  crossorigin="anonymous"></script>

<link rel="stylesheet" href="{{ site.baseurl }}/assets/vallenato/vallenato.css">
<script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-MML-AM_CHTML' async></script>
<script src="{{ site.baseurl }}/assets/vallenato/vallenato.js"></script>


<h3>Carbonara</h3>
<p>
	Carbonara details.
</p><p>
	Carbonara link.
</p><p>
	Carbonara paper.
</p>

<h3>Writhe</h3>
<p>
  Writhe details.
</p><p>
	Writhe link.
</p><p>
	Writhe paper.
</p>
<div class="vallenato">
<h2 style="text-align: center;">Publications</h2>
<div class="vallenato-header" id="su2_center_vortices">
SWRITHE: a python package to identify surprising protein tertiary structure relationships and aid new structure search.
</div><!--/.vallenato-header-->
	
<div class="vallenato-content">
<p>with <a href="[[https://sites.google.com/view/jeffreygiansiracusa/home](https://www.maths.dur.ac.uk/users/christopher.prior/)](https://www.maths.dur.ac.uk/users/christopher.prior/)">Chris Prior</a> and <a href="[[http://pyweb.swan.ac.uk/~pybl/](https://www.diamond.ac.uk/Instruments/Soft-Condensed-Matter/small-angle/B21/Staff/Robert-Rambo.html)](https://www.diamond.ac.uk/Instruments/Soft-Condensed-Matter/small-angle/B21/Staff/Robert-Rambo.html)">Rob Rambo</a>.</p>

<p>We present fast and simple-to-implement measures of the entanglement of protein tertiary structures which are appropriate for highly flexible structure comparison.
   These quantities are based on the writhing and crossing numbers heavily utilised in DNA topology studies. 
   Here we show how they can be applied in a novel manner across various scales of the protein’s backbone to identify similar topologies which can be missed by more common RMSD, secondary structure or primary sequence based comparison methods. 
   We derive empirical bounds on the entanglement implied by these measures and show how they can be used to constrain the search space of a protein for solution scattering, a method highly suited to determining the likely structure of proteins in solution where crystal structure or machine learning based predictions often fail to match experimental data. 
   In addition we identify large scale helical geometries present in a large array of proteins which are consistent across a number of different protein structure types and sequences.
   This is used in one specific case to demonstrate significant structural similarity between Rossmann fold and Tim Barrel proteins, a link which is potentially significant as attempts to engineer the latter have in the past produced the former. 
   Finally we introduce the SWRITHE python package to calculate these metrics and analyse their findings.
</p>
<p><a href="">Publisher</a>, <a href="">arXiv</a>.</p>
</div><!--/.vallenato-content-->
 
</div><!--/.vallenato-->

<div class="vallenato">
<h2 style="text-align: center;">Theses</h2>
<div class="vallenato-header">
PhD Thesis:
</div><!--/.vallenato-header-->

<div class="vallenato-content">
<p> ... </p>
</div><!--/.vallenato-content-->	
	
<div class="vallenato-header">
Masters Dissertation: 
</div><!--/.vallenato-header-->

<div class="vallenato-content">
<p> ... </p>

<p>Submitted in April 2020.</p>
</div><!--/.vallenato-content-->
  
</div><!--/.vallenato-->

<script>
$(document).ready(function() {
	vallenato();
});
</script>
