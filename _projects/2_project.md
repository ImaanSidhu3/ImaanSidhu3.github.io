---
layout: page
title: Turbulent Flow Final Project
description: My final project for Turbulence Theory and Modeling
img: assets/img/Turbulence_Fig1.jpg
importance: 2
category: Academic
giscus_comments: false
---

The focus of this project was to examine two wall-bounded flows with different Reynolds numbers (ratios of viscous to non-viscous forces). The main parameters used to compares the flows were turbulent kinetic energy (TKE) and mean velocity spectra. The goal was to show the difference in energy transfer from laminar to turbulent flow across different length scales. 

TKE quantifies the intensity of velocity fluctuations and describes the energy distribution across the scales of motion. The TKE production term represents the rate of energy transfer from mean velocity gradients to turbulent fluctuations. By analyzing this term, the effects of production in the energy cascades can be determined. The TKE transport term represents the transfer of energy from one region of flow to the other. It is relevant in this problem to describe how energy transfers between the near-wall region and the outer region. Using the turbulent kinetic energy production and transport terms, information can be determined on the energy transfer within the flow and applications of Kolmogorov theory to these wall-bounded flows.

Attached below is an abridged description of my the results from my analysis. The simulation and computation was done in MATLAB. First is a colormap of the flow within the first dataset that describes the flow distribution at various planes.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Turbulence_Fig1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Turbulence_Fig2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Turbulence_Fig3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Colormaps of the flow in Dataset 1
</div>


The figures below show the TKE production term across inner units. This displays the rate at which laminar flow transfers to turbulent flow as it moves along the wall. The peak shows where the most eddies are generated, before a trough when the flow reaches the wall.

<div class="row justify-content-sm-center">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/Turbulence_Fig4.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/Turbulence_Fig5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    TKE
</div>
