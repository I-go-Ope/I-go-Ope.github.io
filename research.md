---
layout: default
title: Research
---

# Research

My research combines **experimental particle physics**, **particle astrophysics**, and **scientific instrumentation** to investigate fundamental questions in high-energy physics. My work integrates large-scale Monte Carlo simulations, detector development, statistical analysis, and scientific computing.

As an undergraduate at Elmhurst University, I contributed to both computational and experimental research through the **Pacific Ocean Neutrino Experiment (P-ONE)** and a study of **ultra-high-energy cosmic-ray composition** using CORSIKA.

---

# Research Snapshot

| Project | Status |
|---------|--------|
| 🟢 Ultra-High-Energy Cosmic-Ray Composition | Active |
| 🟢 Cherenkov Radiation Simulations | Active |
| 🔵 Pacific Ocean Neutrino Experiment | Completed Contribution |

---

# Research Philosophy

I am particularly interested in research that combines computational modeling with experimental measurement. I enjoy developing and working with instrumentation that improves our ability to observe physical phenomena while using simulation and statistical analysis to interpret experimental results.

My long-term interests lie in large collaborative experiments studying cosmic rays, neutrinos, and other high-energy particles, where detector development, scientific computing, and experimental measurements work together to address fundamental questions in particle astrophysics.

---

# Composition of Ultra-High-Energy Cosmic Rays

## Scientific Motivation

Ultra-high-energy cosmic rays are among the most energetic particles observed in nature, yet their composition and astrophysical origins remain uncertain.

When a cosmic ray enters Earth's atmosphere, it interacts with atmospheric nuclei and produces an extensive air shower containing large numbers of secondary particles. Because the original primary particle is no longer directly observable after this interaction, properties of the resulting shower must be used to infer the identity of the primary cosmic ray.

One of the most important composition-sensitive observables is the atmospheric depth at which the shower reaches its maximum particle population, known as the depth of shower maximum, or $X_{\max}$.

This research investigates how $X_{\max}$ and muon production vary with primary energy and atomic species and whether these observables can be used to distinguish between different cosmic-ray primaries.

---

## Research Questions

- How does $X_{\max}$ vary with primary energy?
- How does $X_{\max}$ vary with atomic number?
- How strongly do the $X_{\max}$ distributions of neighboring species overlap?
- How does muon production vary with primary species and energy?
- Can combined shower observables improve primary-composition identification?
- Can Cherenkov radiation provide an additional composition-sensitive observable?

---

## Methods

Air showers were simulated using **CORSIKA 7.8050**.

The simulation set contains primary nuclei ranging from hydrogen through iron across multiple primary energies. Longitudinal shower profiles were processed and analyzed to extract shower-development information and compare trends between primary species.

### Computational Tools

- CORSIKA 7.8050
- Python
- Jupyter Notebook
- NumPy
- SciPy
- Matplotlib
- Gaussian fitting
- Shapiro-Wilk statistical testing
- Automated processing of CORSIKA `.long` files
- Statistical comparison of shower populations

---

# All Charged Particle Analysis

The all-charged-particle longitudinal profile provides a measure of the overall development of each simulated extensive air shower.

For each simulated shower, the depth of maximum charged-particle production was identified and used as the shower's $X_{\max}$ value.

---

## Mean $X_{\max}$

<img class="research-image"
     src="/xmax_mean_heatmap.png"
     alt="Mean Xmax heatmap">

<p class="figure-caption">
Mean simulated Xmax as a function of primary atomic species and energy.
</p>

The mean $X_{\max}$ values show systematic dependence on both primary energy and atomic species. Higher-energy primaries generally develop deeper in the atmosphere, while heavier nuclei tend to reach shower maximum at smaller atmospheric depths.

These trends agree with the expected behavior of extensive air showers and provide a statistical method for distinguishing broad primary-mass groups.

---

## Standard Deviation of $X_{\max}$

<img class="research-image"
     src="/xmax_std_heatmap.png"
     alt="Standard deviation of Xmax heatmap">

<p class="figure-caption">
Standard deviation of simulated Xmax values for each primary species and energy.
</p>

The standard deviation of $X_{\max}$ characterizes the shower-to-shower fluctuations associated with each primary species.

These fluctuations are important because composition measurements depend not only on differences in mean shower depth but also on the width and overlap of the corresponding distributions.

---

## Species Comparison

<img class="research-image"
     src="/shower_depth_plot.png"
     alt="Xmax species and energy comparison">

<p class="figure-caption">
Ranges of Xmax for each simulated primary species at four primary energies.
</p>

This figure compares the range of $X_{\max}$ values for each simulated atomic species across four primary energies.

Although systematic trends with energy and atomic number are visible, substantial overlap remains between neighboring elemental species.

This overlap demonstrates one of the major limitations of using $X_{\max}$ alone for event-by-event primary identification and motivates the investigation of additional composition-sensitive observables.

---

# Muon Analysis

Muon production provides a complementary observable to the overall charged-particle shower profile.

Because muons are primarily produced through the hadronic component of the air shower, their distributions may contain additional information about the mass and energy of the primary cosmic ray.

The total muon population was determined by combining positively and negatively charged muons within each longitudinal shower profile.

---

## Mean Muon Distribution

<img class="research-image"
     src="/mu_xmax_combined_heatmap.png"
     alt="Mean total muon heatmap">

<p class="figure-caption">
Mean total muon observable as a function of primary atomic species and energy.
</p>

The mean muon distributions show systematic changes with both primary energy and atomic species.

Compared with the all-charged-particle $X_{\max}$ distributions, the muon observables provide a different view of shower development and may offer complementary information for primary-composition studies.

---

## Standard Deviation of Muon Distribution

<img class="research-image"
     src="/mu_xmax_std_heatmap.png"
     alt="Standard deviation of total muon heatmap">

<p class="figure-caption">
Standard deviation of the total muon observable for each simulated primary species and energy.
</p>

The standard deviation heatmap shows the shower-to-shower variability of the muon observable.

Understanding these fluctuations is necessary when evaluating how effectively muon information can distinguish neighboring primary species.

---

## Muon Species Comparison

<img class="research-image"
     src="/mu_total_error_overlay.png"
     alt="Muon species comparison">

<p class="figure-caption">
Comparison of total muon distributions across primary species and four simulated energies.
</p>

The species-comparison plot illustrates how the muon distributions change with primary species and energy while also showing the degree of overlap between neighboring nuclei.

Together with $X_{\max}$, these results motivate the use of multiple shower observables when attempting to infer cosmic-ray composition.

---

# Cherenkov Radiation Extension

I am currently extending this research to investigate **Cherenkov radiation produced during extensive air showers**.

The goal is to determine whether Cherenkov observables provide additional sensitivity to primary cosmic-ray composition when combined with $X_{\max}$ and muon measurements.

Current work includes configuring CORSIKA for Cherenkov production, testing simulation parameters, developing automated simulation workflows, and determining how Cherenkov information can be correlated with shower development.

---

# Current Status

- ✔ Initial CORSIKA simulation dataset completed
- ✔ Hydrogen-through-iron species analysis completed
- ✔ Automated `.long` file processing developed
- ✔ All-charged-particle $X_{\max}$ analysis completed
- ✔ Muon analysis completed
- ✔ Statistical analysis completed
- ✔ Mean and standard-deviation heatmaps produced
- ✔ Species-comparison plots produced
- ✔ Research poster completed
- ✔ Senior research presentation completed
- 🔄 Expanded simulation statistics underway
- 🔄 Cherenkov simulation development underway
- 🔄 Manuscript in preparation

---

# Research Outputs

<a class="button-link" href="#">
📄 Paper (Coming Soon)
</a>

<a class="button-link"
   href="/Composition%20of%20Ultra-High-Energy%20Cosmic%20Rays.pdf">
🖼 Research Poster
</a>

<a class="button-link"
   href="https://github.com/I-go-Ope/Ultra-High-Energy-Cosmic-Rays-UHECRs-">
💻 Project Repository
</a>

---

# Pacific Ocean Neutrino Experiment (P-ONE)

*(Timing-system electronics photograph coming soon)*

From 2024–2025, I contributed to the development, testing, and deployment of the central timing system for the **Pacific Ocean Neutrino Experiment (P-ONE)**.

P-ONE is a deep-ocean neutrino telescope being developed in the Pacific Ocean. Precise timing between detector components is necessary for reconstructing the arrival times and trajectories of particles produced by neutrino interactions.

My work focused on detector instrumentation, timing-system integration, system validation, and technical documentation supporting the experiment's detector-development efforts.

## My Contributions

- Integrated and tested components of the central timing system
- Performed timing-system calibration and validation
- Assisted with detector-system integration
- Supported testing of timing and signal pathways
- Contributed to technical documentation
- Designed supporting instrumentation for laboratory operation and deployment

My detector-development work contributed to peer-reviewed journal publications, conference proceedings, invited presentations, and research posters associated with the P-ONE collaboration.

<a class="button-link"
   href="/publications.html">
View P-ONE Publications and Presentations
</a>

---

# Current Research Directions

My current research efforts are focused on

- Expanding CORSIKA simulation statistics
- Improving automated simulation workflows
- Investigating Cherenkov radiation as an additional composition-sensitive observable
- Developing additional statistical methods for primary-particle classification
- Comparing multiple shower observables for cosmic-ray composition studies

More broadly, I am interested in experimental particle physics and particle astrophysics involving **cosmic rays, high-energy neutrinos, detector instrumentation, optical and radio detection techniques, and large international experimental collaborations**.
