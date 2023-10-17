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
	Much of my work has been based on the development of a <a href="https://pubs.acs.org/doi/10.1021/acs.jctc.9b01010">software for ab-initio structure prediction from BioSAXS data.</a> Biological small angle X-ray scattering is a technique for determining protein structures in solution which is useful for proteins which fail to crystallise or are too large for NMR. The original model used a novel constrained backbone algorithm to randomly search the space of possible conformations in order to fit experimental scattering data. This algorithm uses local geometric constraints on the backbone which are analogous to the Ramachandran distributions of dihedral angles. Though these constraints ensure the predicted structures are locally realistic, the global fold may not be. By studying the distribution of entanglement across the PDB, we are able to include a penalty for unrealistic global entanglement. This massively reduces the search space of possible conformations, and ensures the output structures are realistic and behave well in MD simulations. The full carbonara software package will be released for public soon, but if you have scattering data that you would like to study in the meantime please do contact us!
</p>

<h3>Writhe</h3>
<p>
	To study the entanglement of protein backbone curves we use the writhe. This is a topological quantity which measures the amount of self entanglement of a curve. This quantity has a wide range of uses, from solar physics to DNA biology. To compute this, imagine your curve is projected onto a plane. There will be points where it passes over itself, which we call crossings. We give each crossing a sign using the below convention. The signed sum of crossings will be dependent on the angle of projection, so the writhe is an average of the signed sum of crossings over all possible projections.
	<p float="left">
		<img align="top" src="{{ site.baseurl }}/files/positive.png" width="10%" hspace="20px"/>
		<img align="top" src="{{ site.baseurl }}/files/negative.png" width="10%" hspace="20px"/>
		<img align="top" src="{{ site.baseurl }}/files/trefoil_writhe.png" width="50%" hspace="75px"/>
	</p>
In my work, I use the writhe in the Carbonara software to restrict predictions to biologically realistic conformations. To determine what is realistic, we compute the writhe of a representative sample of proteins from the PDB, and found a clear lower bound on the entanglement as a function of the number of secondary structure elements of a protein. By studying the distribution of writhe across the PDB, we also uncovered some interesting families of proteins. Firstly, there are proteins which come close to achieving, or even beating, the linear upper bound on writhe. We see that this is due to their large scale helical structure, and have found that this is linked to structural stability for proteins. The second family of proteins we are interested in are those which have quite complex entanglement yet net zero writhe. This idea was inspired by a method of storing cables used by roadies/sound engineers, where the cable is looped up without ever becoming knotted. In terms of writhe, this is due to orientation of the loops, where there is essentially cancellation in the entanglement between each loop. We have uncovered a large set of proteins which have a writhe profile that matches this conformation, which we are currently calling roadie proteins. There are many physical uses for this conformation in other contexts, but its functional advantage in proteins is not yet clear to us. Please do get in touch if you have any ideas! For the full details of this work, see the preprint below. Alongside this paper, we provide an <a href="[https://colab.research.google.com/github/arronelab/SWRITHE/blob/main/SWRITHE.ipynb](https://github.com/arronelab/SWRITHE)">iPython notebook</a> where you can study the writhe profile of your favourite protein, and search for its helical or roadie substructures
</p>
<div class="vallenato">
<h2 style="text-align: center;">Publications</h2>
<div class="vallenato-header" id="su2_center_vortices">
The SKMT Algorithm: A method for assessing and comparing underlying protein entanglement. (Preprint)
</div><!--/.vallenato-header-->
	
<div class="vallenato-content">
<p>with <a href="[[https://sites.google.com/view/jeffreygiansiracusa/home](https://www.maths.dur.ac.uk/users/christopher.prior/)](https://www.maths.dur.ac.uk/users/christopher.prior/)">Chris Prior</a> and <a href="[[http://pyweb.swan.ac.uk/~pybl/](https://www.diamond.ac.uk/Instruments/Soft-Condensed-Matter/small-angle/B21/Staff/Robert-Rambo.html)](https://www.diamond.ac.uk/Instruments/Soft-Condensed-Matter/small-angle/B21/Staff/Robert-Rambo.html)">Rob Rambo</a>.</p>

<p>We present fast and simple-to-implement measures of the entanglement of protein tertiary structures which are appropriate for highly flexible structure comparison. These are performed using the SKMT algorithm, a novel method of smoothing the alpha-carbon backbone to achieve a minimal complexity curve representation of the manner in which the protein's secondary structure elements fold to form its tertiary structure. Its subsequent complexity is characterised using measures based on the writhe and crossing number quantities heavily utilised in DNA topology studies, and which have shown promising results when applied to proteins recently. The SKMT smoothing is used to derive empirical bounds on a protein's entanglement relative to its number of secondary structure elements. We show that large scale helical geometries dominantly account for the maximum growth in entanglement of protein monomers, and further that this large scale helical geometry is present in a large array of proteins, consistent across a number of different protein structure types and sequences. We also show how these bounds can be used to constrain the search space of protein structure prediction from small angle x-ray scattering experiments, a method highly suited to determining the likely structure of proteins in solution where crystal structure or machine learning based predictions often fail to match experimental data. Finally we develop a structural comparison metric based on the SKMT smoothing which is used in one specific case to demonstrate significant structural similarity between Rossmann fold and TIM Barrel proteins, a link which is potentially significant as attempts to engineer the latter have in the past produced the former. We provide the SWRITHE interactive python notebook to calculate these metrics.
</p>
<p><a href="">Publisher</a>, <a href="https://www.biorxiv.org/content/10.1101/2023.06.09.544297v1">BiorXiv</a>.</p>
</div><!--/.vallenato-content-->
</div><!--/.vallenato-->

<script>
$(document).ready(function() {
	vallenato();
});
</script>
