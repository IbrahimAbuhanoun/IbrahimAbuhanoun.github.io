---
title: "Master's Degree Experience"
excerpt: "The objective of my master's work was to improve the design of a soft robot design concept called a Vine Robot and test its navigation capability in a simulated jet engine environment. This helps us determine whether cost-effective soft robots can be a potential substitute to more expensive inspection equipment like borescopes that are more flexible and are able to operate without requiring engine overhauls.<br><video width='700' controls style='display:block;margin:20px auto 0 auto;max-width:100%;'><source src='/Vine_Tube_Motion_With_Bullet_Cap.mp4' type='video/mp4'></video><span style='display:block;text-align:center;'><em><strong>Demonstration of tube navigating the simulated engine environment</strong></em></span>"
collection: portfolio
---
<style>
  .research-figure-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 28px;
    align-items: start;
    margin: 30px auto;
    width: 100%;
  }

  .research-figure {
    margin: 0;
    text-align: center;
    min-width: 0;
  }

  .research-media {
    width: 100%;
    height: 320px;
    display: block;
    border-radius: 8px;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.15);
  }

  .research-photo {
    object-fit: cover;
  }

  .research-diagram {
    object-fit: contain;
    background-color: #fff;
  }

  .research-caption {
    margin-top: 10px;
    padding: 0 8px;
    color: #000;
    font-size: 1.03rem;
    font-weight: bold;
    font-style: italic;
    line-height: 1.35;
    text-align: center;
  }

  @media (max-width: 700px) {
    .research-figure-grid {
      grid-template-columns: 1fr;
    }

    .research-media {
      height: auto;
      max-height: 320px;
    }
  }
</style>

## Background & Motivation

Engines operating in particle-dense environments (like sand or dust) suffer structural damage over time. Traditional inspection tools — borescopes — are rigid, limited in reach, and expensive (up to **$84,000**). Soft robots offer a cheaper, more flexible alternative that could eliminate long engine overhauls and reach critical areas for research and diagnostics.

<div class="research-figure-grid">

  <figure class="research-figure">
    <img
      src="/images/Osprey_In_Sand.jpg"
      alt="V-22 Osprey operating in a sand-dense environment"
      class="research-media research-photo">
    <figcaption class="research-caption">
      V-22 Osprey engines operating in a sand-dense environment
    </figcaption>
  </figure>

  <figure class="research-figure">
    <img
      src="/images/Sand_Deposits.jpg"
      alt="Sand deposits on the last-stage power turbine of an M250 engine"
      class="research-media research-photo">
    <figcaption class="research-caption">
      Sand deposits on the last-stage power turbine of an M250 engine
    </figcaption>
  </figure>

</div>

## What Is a "Vine Robot"?

A vine robot is a **tip-growing soft continuum robot**: pressurized air everts the material at the tip — turning it inside-out, much like a folded sock unrolling — to extend the body outward. This growth mechanism offers several advantages over traditional borescopes:

- **No wall friction.** Since translation energy is concentrated entirely at the tip, the tube body remains static relative to its surroundings, eliminating the sliding friction borescopes rely on to advance — and the jamming risk that friction-based locomotion introduces.
- **Fully flexible body.** Unlike borescopes, which are only flexible near the tip, a vine robot's entire length remains compliant, allowing it to conform to complex, cluttered geometries.
- **Extreme compressibility.** Vine robots can deform to roughly ¼ their original diameter, enabling access through narrower gaps that rigid tools like borescopes cannot reach.

<div class="research-figure-grid">

  <figure class="research-figure">
    <img
      src="/images/Vine_Robot.jpg"
      alt="Components and structure of a vine robot"
      class="research-media research-diagram">
    <figcaption class="research-caption">
      Components and structure of a "Vine Robot"
    </figcaption>
  </figure>

  <figure class="research-figure">
    <video
      autoplay
      muted
      loop
      playsinline
      preload="auto"
      controls
      class="research-media research-photo">
      <source src="/Borescope_Function.mp4" type="video/mp4">
    </video>
    <figcaption class="research-caption">
      Demonstration of borescope functionality and limited flexibility
    </figcaption>
  </figure>

</div>
## Previous Work

A proof-of-concept vine robot was developed for the 2024 senior capstone project, but the design had two key limitations that this work aimed to address:

- **Unrealistic engine model.** The axial compressor section was oversized and geometrically inaccurate to the M250 engine, limiting the relevance of navigation testing.
- **Constrained tube dimensions.** Tube length was capped by the heat sealer's working length, and diameters below 1 inch could not be reliably fabricated — concentrated heat from the sealing process caused pinholes in the tube wall, compromising structural integrity.
- **Impaired navigation.** The tube's flat tip geometry caused it to deform around and conform tightly against compressor blades, restricting further advancement.

<div class="research-figure-grid">

  <figure class="research-figure" style="flex:1.2;">
    <img
      src="/images/Big_Gap_Model.jpg"
      alt="Original proof-of-concept engine model"
      style="width:100%;
             height:auto;
             border-radius:8px;
             display:block;
             box-shadow:0 3px 10px rgba(0,0,0,0.15);">
    <figcaption class="research-caption">
      Oversized initial axial compressor model of the M250 engine
    </figcaption>
  </figure>

  <figure class="research-figure" style="flex:0.8;">
    <img
      src="/images/Trad_Heatslr.jpg"
      alt="Heat sealer length limitation"
      style="width:100%;
             height:auto;
             border-radius:8px;
             display:block;
             box-shadow:0 3px 10px rgba(0,0,0,0.15);">
    <figcaption class="research-caption">
      Traditional impulse heat sealer with 20" of working length
    </figcaption>
  </figure>

</div>
