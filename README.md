# The Banff Bunny Project: Benchmarks for Open Cortical Microtubule Simulations

Simulations are an increasingly popular method of modelling cortical microtubule (CMT) systems. While the field has benefitted from the diversity of approaches, there is difficulty in understanding how each model compares and sources of differences among  models. The aim of this project is to increase accessibility, reproducibility, interpretability, and understanding simulation consistency. This project arose from two workshops:
- Lorentz 4-Day Workshop on [Modelling plant cortical microtubules](https://www.lorentzcenter.nl/modelling-plant-cortical-microtubules.html), Leiden, the Netherlands (2025)
- Banff International Research Station 5-Day Workshop on [Modelling of Plant Microtubules](https://www.birs.ca/events/2026/5-day-workshops/26w5658), Banff, Canada (2026)

<p align="center">
  <img src="./realBanffBunny.jpg" alt="Real Banff bunny" width="300">
  <img src="bunny_corticalsim3D.png" alt="Description of second image" width="205">
  <br>
  <em>Figure 1. Inspired by the Stanford Bunny, we seek to provide a similar benchmark for CMT simulations: the Banff Bunny. Left: a real life Banff bunny found in Banff. Picture taken by Eva Deinum. Right: simulation of CMTs on a bunny using CorticalSim3D by Bandan Chakrabortty and Ashlin Raj.</em>
</p>

## Goals
1. Provide a benchmark for simulation comparison and standardization.
2. Determine and understand the sources for differences between simulation predictions.
3. Increase accessibility by providing open source software and publicly available data.

## Simulation Frameworks Involved:
- CorticalSim (Eva Deinum)
- CorticalSim3D (Bandan Chakrabortty, Ashlin Raj)
- TimSim (Tim Tian)
- Tubulaton (Tamsin Spelman, Henrik Jönsson)

## Current Work
This is ongoing work! We hope to have more results shortly.

We are currently developing benchmarks for comparing CorticalSim, CorticalSim3D, and TimSim. The parameter set used is the default parameter set in the [methods paper for CorticalSim](https://doi.org/10.3389/fphy.2014.00019). The geometries used so far are a periodic plane ($80\times80$ microns) and cylinder with $100\%$ edge-induced catastrophe (radius $R=20$ and height $h=40$ microns).

Simulation outputs: CSV of 100 runs. First column is the time step (1 min). Subsequent columns are measured quantities for a given random seed, at each time step. Measured quantities are:
- MT length averaged over all MTs at each time
- MT density at each time
- Order parameters at each time (see above paper)
  - $S_2$ anisotropy 
  - $\Omega$ dominant angle

Data and more info to follow soon.
<!-- ### Directories

Each geometry is given a directory. Within a geometry directory, the separate subdirectories contain outputs of each simulation. Not all simulations have been run for all geometries yet.

```text
./
├── 80x80_periodic_plane/
│   ├── corticalsim/
│   └── timsim/
└── cylinder_20/
    ├── corticalsim/
    ├── corticalsim3d/
    └── timsim/
``` -->
## Get Involved!
Are you working on a CMT simulation? Feel free to contact any of us, compare outputs, and contribute!