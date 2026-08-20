---
title: "Electrothermal & Heat Transfer Analysis Using COMSOL Multiphysics"
excerpt: "This section showcases COMSOL Multiphysics projects exploring electrothermal coupling, heat transfer, and the influence of material properties on temperature distributions."
collection: portfolio
---
## Project Overview
### Copper Bus Bar Problem
The objective of this study was to examine the electrothermal behavior of a copper bus bar (with three titanium bolts) under a specified temperature constraint. Specifically, the goal was to determine the maximum voltage that could be applied across the bus bar without its temperature exceeding 350 K.
### Unit Circle Problem
The objective of this study was to investigate the effect of material selection on the thermal behavior of a unit circle. The analysis compared the resulting temperature profiles for three different materials: gold, lead, and helium gas.
## Design Methodology
### Copper Bus Bar Design Methodology 
- **Parametric Sweep:** A parametric sweep was set over an appropriate voltage range (20-30 mV) to identify the maximum voltage required to meet the temperature constraint.
- **Plot Adjustments:** The maximum temperature was set for both the bus bar body and for the scale, and the bus bar (green) was selected as the testing domain for the simulation.

<div class="research-figure-grid" style="grid-template-columns: 1fr; margin-top:20px;">
  <figure class="research-figure" style="max-width:700px; margin:0 auto; width:100%;">
    <img
      src="/images/COMSOL/Param_Sweep.jpg"
      alt="Parametric sweep setup for voltage range"
      style="width:100%;
             height:auto;
             display:block;
             border-radius:8px;
             box-shadow:0 3px 10px rgba(0,0,0,0.15);"
    >
    <figcaption class="research-caption" style="text-align:center; width:100%; color:#000; font-weight:bold; font-style:italic;">
      Demonstration of a parametric sweep configured to test voltages from 20–30 mV
    </figcaption>
  </figure>
</div>

<div class="research-figure-grid" style="grid-template-columns: 1fr; margin-top:20px;">
  <figure class="research-figure" style="max-width:700px; margin:0 auto; width:100%;">
    <img
      src="/images/COMSOL/Plot_Adj.jpg"
      alt="Plot adjustments to track the 350 K constraint"
      style="width:100%;
             height:auto;
             display:block;
             border-radius:8px;
             box-shadow:0 3px 10px rgba(0,0,0,0.15);"
    >
    <figcaption class="research-caption" style="text-align:center; width:100%; color:#000; font-weight:bold; font-style:italic;">
      Demonstration of plot adjustments before simulating the bus bar model: The temperature bounds were set and shown, and the bus bar (green) was selected as the domain
    </figcaption>
  </figure>
</div>

### Unit Circle Design Methodology 
- **Defining Material Properties:** The relevant material and thermal properties were defined for each of the gold, lead, and the helium gas unit circle designs. Namely, the material density, specific heat capacity and the thermal conductivity values were modified.
- **Setting a Heat Source & BCs:** For each unit circle, the Neumann and the Dirichlet boundary conditions were set identically according to the chart below.

<div class="research-figure-grid" style="grid-template-columns: 1fr; margin-top:20px;">
  <figure class="research-figure" style="max-width:700px; margin:0 auto; width:100%;">
    <img
      src="/images/COMSOL/Def_Mats.jpg"
      alt="Material definitions for gold, lead, and helium models"
      style="width:100%;
             height:auto;
             display:block;
             border-radius:8px;
             box-shadow:0 3px 10px rgba(0,0,0,0.15);"
    >
    <figcaption class="research-caption" style="text-align:center; width:100%; color:#000; font-weight:bold; font-style:italic;">
      Demonstration of thermal and material properties defined for each material — gold, lead, and helium — applied to the full geometry
    </figcaption>
  </figure>
</div>

<div class="research-figure-grid" style="grid-template-columns: 1fr; margin-top:20px;">
  <figure class="research-figure" style="max-width:700px; margin:0 auto; width:100%;">
    <img
      src="/images/COMSOL/Heat_Src_BC.jpg"
      alt="Heat source and boundary conditions applied to the unit circle"
      style="width:100%;
             height:auto;
             display:block;
             border-radius:8px;
             box-shadow:0 3px 10px rgba(0,0,0,0.15);"
    >
    <figcaption class="research-caption" style="text-align:center; width:100%; color:#000; font-weight:bold; font-style:italic;">
      Demonstration of Neumann and Dirichlet boundary conditions applied for all three material models
    </figcaption>
  </figure>
</div>
