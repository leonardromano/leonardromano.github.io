---
title: "Gadget4-Osaka — A framework for physical realism in large-scale simulations"
permalink: /research/g4-osaka/
author_profile: true
---

**Gadget4-Osaka** is a customised version of the cosmological SPH code [Gadget-4](https://wwwmpa.mpa-garching.mpg.de/gadget4/), designed to follow the full **life cycle of interstellar dust** in galaxy-scale simulations.  
It couples state-of-the-art models for **grain-size evolution** with a detailed treatment of gas-phase chemistry.  
This allows us to track how dust and molecular gas evolve in different galactic environments — from dense star-forming clouds to diffuse halo gas — while keeping the simulations physically realistic.

A key strength of Gadget4-Osaka is its great interoperability with [SKIRT](https://skirt.ugent.be/root/_home.html) to produce realistic **synthetic observables** — maps and spectra of dust and molecular gas — that can be directly compared to telescope data from ALMA, Herschel, and JWST.  
By bridging simulations and observations, it helps us understand how dust shapes galaxy evolution across cosmic history.

Gadget4-Osaka powers the [CROCODILE](https://sites.google.com/view/crocodilesimulation/home) cosmological simulation suite, which follows the formation and evolution of galaxies across the history of the Universe. In CROCODILE, Gadget4-Osaka combines detailed for gas chemistry and cooling, star formation, stellar explosions, and black hole growth, allowing us to explore how small-scale processes shape galaxies on cosmic scales. Future CROCODILE studies will explore the evolution of dust grain-sizes across cosmic times.

The projects involving Gadget4-Osaka are community-driven efforts involving many experts in dust- and chemistry modelling, observational data analysis and numerical simulations.
I acknowledge the support from my colleagues and close collaborators Kosei Matsumoto, [Yuri Oku](https://www.yurioku.com/), Monica Relaño, [Stefan van der Giessen](https://www.linkedin.com/in/stefan-van-der-giessen-9928a0182/?originalSubdomain=be), [Kentaro Nagamine](https://astro-osaka.jp/kn/), Ilse De Looze, Hiroyuki Hirashita, and many others who contributed to this work.

Below are some highlights from our project.

## Modeling the Galactic Dust Life Cycle

<div style="display: flex; flex-wrap: wrap-reverse; align-items: center; margin-bottom: 40px;">

  <div style="flex: 1; min-width: 280px; padding-right: 20px;">
    <h3 style="margin-top: 0;">Following Grains from Birth to Destruction</h3>
    <p>
      In Gadget4-Osaka, each gas particle carries information on its dust mass and the full <strong>grain-size distribution</strong>.  
      The code models key physical processes: dust growth by accretion of metals in dense gas, shattering in high-speed grain–grain collisions, coagulation in molecular clouds, thermal sputtering in hot plasma, and destruction by supernova shocks.
    </p>
    <p>In a <a href="https://ui.adsabs.harvard.edu/abs/2022MNRAS.514.1441R/abstract" target="_blank" rel="noopener">key publication</a> we showed how a major shortcoming of particle based methods such as SPH is the lack of mixing between fluid tracers. We addressed this, by adding <strong>numerical diffusion</strong> of dust and metals between particles, which strongly affected grain-size evolution.</p>
    
    <p>
      This framework lets us study how dust evolves across galactic environments (e.g. <a href="https://ui.adsabs.harvard.edu/abs/2022MNRAS.515.5306R/abstract" target="_blank" rel="noopener">Relaño et al. 2022</a>, <a href="https://ui.adsabs.harvard.edu/abs/2024A%26A...692A..39V/abstract" target="_blank" rel="noopener">van der Giessen et al. 2024</a>), under a broad range of different star-formation and feedback conditions.  
      The inclusion of size distributions means we can predict wavelength-dependent extinction and emission directly from the simulations.
    </p>
  </div>

  <div style="flex: 1; min-width: 280px; padding-left: 20px;">
    <img src="/images/projects/g4-osaka/dust_slice.png" alt="Density-weighted projection of large-grain abundance." style="width: 100%; border-radius: 8px;">
  </div>
</div>

## How Environment Shapes Dust and Molecular Gas

<div style="display: flex; flex-wrap: wrap; align-items: center; gap: 2rem;">

  <div style="flex: 1; min-width: 300px;">
    <img src="/images/projects/g4-osaka/H2_map.png" alt="Map of molecular-gas surface-density" style="width: 100%; border-radius: 8px;">
  </div>

  <div style="flex: 1; min-width: 300px;">

<h3>Dust Survival in Different Galactic Neighborhoods</h3>

<p>
Gadget4-Osaka simulations reveal strong variation in <strong>dust abundance</strong> and <strong>molecular gas fraction</strong> across a galaxy.  
Dense spiral arms can be rich in both, while feedback-heated regions — particularly near young star clusters — show significant dust destruction.
</p>

<p>
The <a href="https://ui.adsabs.harvard.edu/abs/2022MNRAS.514.1461R/abstract" target="_blank" rel="noopener">coupling of dust physics and H₂ chemistry</a> allows us to explore how galactic structure and feedback regulate the cold ISM.  
We find that feedback-driven turbulence and shocks are key in determining where dust can survive long enough to seed molecular cloud formation.
</p>

  </div>
</div>

## From Simulation to Observation: Synthetic Dust and Gas Maps

<div style="display: flex; flex-wrap: wrap-reverse; align-items: center; margin-bottom: 40px;">

  <div style="flex: 1; min-width: 280px; padding-right: 20px;">
    <h3 style="margin-top: 0;">Turning Models into “Virtual Telescopes”</h3>
    <p>
      Gadget4-Osaka outputs can be post-processed (<a href="https://ui.adsabs.harvard.edu/abs/2024A%26A...689A..79M/abstract" target="_blank" rel="noopener">Matsumoto et al. 2024</a>) to create synthetic maps in the far-infrared, submillimetre, and molecular line emission (e.g. CO).  
      By matching resolution and noise to real instruments, we can perform direct, quantitative comparisons with ALMA, Herschel, and JWST data.
    </p>
    <p>
      This approach makes it possible to test dust models against observations in a controlled setting, revealing biases in dust mass estimates or CO-to-H₂ conversion factors.
    </p>
  </div>

  <div style="flex: 1; min-width: 280px; padding-left: 20px;">
    <img src="/images/projects/g4-osaka/synthetic_observation.png" alt="Synthetic composite IR maps" style="width: 100%; border-radius: 8px;">
  </div>
</div>

---

(Last modified 08.08.2025)

[← Back to Research Overview](/research/)
