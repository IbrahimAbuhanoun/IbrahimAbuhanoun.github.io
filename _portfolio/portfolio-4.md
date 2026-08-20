---
title: "Electrothermal & Heat Transfer Analysis Using COMSOL Multiphysics"
excerpt: "This section showcases COMSOL Multiphysics projects exploring electrothermal coupling, heat transfer, and the influence of material properties on temperature distributions."
collection: portfolio
---
## Project Overview
### Copper Busbar Problem
The objective of this study was to examine the electrothermal behavior of a copper busbar (with three titanium bolts) under a specified temperature constraint. Specifically, the goal was to determine the maximum voltage that could be applied across the busbar without its temperature exceeding 350 K.
### Unit Circle Problem
The objective of this study was to investigate the effect of material selection on the thermal behavior of a unit circle. The analysis compared the resulting temperature profiles for three different materials: gold, lead, and helium gas.
## Design Methodology
### Copper Bus Bar Design Methodology 
- **Parametric Sweep:** A parametric sweep was set over an appropriate voltage range (20-30 mV) to identify the maximum voltage required to meet the temperature constraint.
- **Plot Adjustments:** The maximum temperature was set for both the busbar body and for the scale, and the busbar (green) was selected as the testing domain for the simulation.

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
      Demonstration of plot adjustments before simulating the busbar model: The temperature bounds were set and shown, and the bus bar (green) was selected as the domain
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
      Demonstration of Neumann and Dirichlet boundary conditions applied for all three material models. Note that the purple section represents a positive heat source application
    </figcaption>
  </figure>
</div>

## Results & Discussion
### Copper Busbar Results
As shown below, the maximum applied voltage that maintains the copper busbar at the specified temperature limit of 350 K is approximately 27.3 mV. This relatively small voltage is reasonable given copper's low electrical resistivity, which allows substantial current to flow even at low applied voltages, resulting in Joule heating. Copper's high thermal conductivity also promotes a relatively uniform temperature distribution across the busbar.
### Unit Circle Results 
As shown below, the relatively high thermal conductivities of gold and lead promote heat transfer away from the heat source, resulting in a more uniform temperature distribution throughout the domain. In contrast, helium has a much lower thermal conductivity, causing heat to remain concentrated near the source and producing a localized high-temperature region.

<div class="research-figure-grid" style="grid-template-columns: 1fr; margin-top:20px;">
  <figure class="research-figure" style="max-width:700px; margin:0 auto; width:100%;">
    <img
      src="/images/COMSOL/Bus_Results.jpg"
      alt="Bus bar simulation results showing maximum voltage and temperature"
      style="width:100%;
             height:auto;
             display:block;
             border-radius:8px;
             box-shadow:0 3px 10px rgba(0,0,0,0.15);"
    >
    <figcaption class="research-caption" style="text-align:center; width:100%; color:#000; font-weight:bold; font-style:italic;">
      Demonstration of the temperature profile of the copper busbar undergoing joule heating. The maximum voltage required to reach the upper temperature limit (350 K) is ~27.3 mV
    </figcaption>
  </figure>
</div>

<div class="research-figure-grid" style="grid-template-columns: 1fr; margin-top:20px;">
  <figure class="research-figure" style="max-width:700px; margin:0 auto; width:100%;">
    <img
      src="/images/COMSOL/Circle_Res.jpg"
      alt="Temperature distribution results for gold, lead, and helium unit circle models"
      style="width:100%;
             height:auto;
             display:block;
             border-radius:8px;
             box-shadow:0 3px 10px rgba(0,0,0,0.15);"
    >
    <figcaption class="research-caption" style="text-align:center; width:100%; color:#000; font-weight:bold; font-style:italic;">
      Demonstration of the temperature profile across the unit circle geometry for gold, lead, and helium gas
    </figcaption>
  </figure>
</div>
