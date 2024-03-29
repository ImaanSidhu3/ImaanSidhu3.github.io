---
layout: page
title: Parker Solar Probe Redesign
description: My senior capstone project at Purdue University
img: assets/img/PSP_cover.jpg
importance: 1
category: Academic
related_publications: false
---


For my senior capstone project at Purdue, a team of fellow aerospace engineers and I designed an updated version of the Parker Solar Probe and created a mission to demonstrate its possible applications. The project involved a complete conceptual overhaul of the probe's technical ability as well as a replanning of the orbital trajectory.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/PSP_mission_design.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image describes our overall mission redesign, accounting for new instrumentation, new propulsion methods, and a new trajectory. 
</div>

The project focused on revamping the Parker Solar Probe with two scienfitic goals: Flying by another planet and achieving a stable orbit of < 0.5 AU. The initial stages of the project focused on choosing which scienfitic instruments would we changed and which planet would achieve the best gravity assist for our probe. 

The trajectory model was written in MATLAB using fixed-point iteration. The parameters included the overall mass, solar sail size, and number of achievable passes around the Sun. The final orbit reached 0.35 AU from the Sun with growing inclination to cover the equator and poles of the Sun. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/PSP_Orbital_Analysis.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image shows the projections of the probe's orbit around the Sun as well as the classical orbital parameters 
</div>


The most important constraint of the project, as with most projects, was the overall budget. Capped at $300M, multiple factors were accounted for including production, launch, communication systems, and various recurring costs. Initial estimates were $291M but the point cost estimate was augmented by a 1,000,000 iteration Monte Carlo simulation based on uncertainties of each cost estimating relationship. The simulation predicted an 82% confidence of the programmatic costs being less than $300M, with a maximum cost overrun estimated to be less than 9% over the target.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/PSP_Monte_Carlo.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image shows the Monte Carlo simulations of the cost model.
</div>

This is a general overview of the project which lasted 6 months. We did additional work on: instrument selection, solar sail modeling, Hohmann transfer calculations, CAD modelling, telemetry and communication estimation, radiation and thermal analysis, power estimation, and attitude and controls. 

Software used: MATLAB, Python, and Solidworks

Techniques used: Pareto Analysis and Monte Carlo Simulations
