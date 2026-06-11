---
title: Research
eyebrow: Research
subtitle: High-fidelity simulation of multiphase flows — solver development, wake dynamics, and the numerics that make both possible.
permalink: /research/
---

<article class="project" id="dns-cylinder">
  <h3>Direct numerical simulation of turbulent air&ndash;water flow past a circular cylinder <span class="tag">Ongoing</span></h3>
  <p class="meta">
    <b>IIT Madras</b>, with Prof. A. Sameen &middot; Jul 2025 &ndash; present<br>
    Re = 100&ndash;300 &middot; 8&ndash;30M cells &middot; six-equation two-fluid model &middot; Fortran &middot; MPI + GPUs (PARAM Shakti, NSM)
  </p>
  <p>
    The core of my current work: resolving the wake of a circular cylinder in a
    compressible air&ndash;water flow without turbulence modelling. Each phase keeps its
    own velocity field, so the solver can capture genuine slip between the gas and the
    liquid &mdash; essential for the droplet&ndash;air interface dynamics that develop in
    the wake. Jobs are distributed one GPU per MPI rank on PARAM&nbsp;Shakti, and the
    immediate task is validation: comparing computed shedding frequencies against
    Strouhal-number data from published DNS and experimental studies before pushing to
    higher Reynolds numbers.
  </p>
  <!-- Figure slot — drop a vorticity/interface render into assets/img/ and uncomment:
  <figure class="fig">
    <img src="{{ '/assets/img/wake-q-criterion.png' | relative_url }}" alt="Instantaneous wake structures behind the cylinder">
    <figcaption><span class="figno">Fig.&thinsp;2</span> &mdash; Your caption here.</figcaption>
  </figure>
  -->
</article>

<article class="project" id="thesis-solver">
  <h3>A compressible multifluid solver for gas&ndash;liquid flow past a bluff body</h3>
  <p class="meta">
    <b>B.Tech thesis</b> &middot; Dec 2024 &ndash; Apr 2025 &middot; carried out at IIT Madras (host: Prof. A. Sameen); thesis guide: Dr. Aldin Justin Sundaraj, KITS<br>
    Six-equation formulation &middot; HLLC-Batten Riemann scheme &middot; unstructured tetrahedral grid, ~4M cells
  </p>
  <p>
    My undergraduate thesis built the foundation the DNS work now stands on: a
    three-dimensional finite-volume solver for compressible gas&ndash;liquid two-phase
    flow, using a six-equation two-fluid model with an HLLC-Batten scheme for the
    interfacial fluxes on unstructured tetrahedra. The solver was validated against the
    benchmark case of Yeom &amp; Chang (2013), with agreement within about one percent,
    and then applied to vortex shedding and interface dynamics around a cylinder at
    low-to-moderate Reynolds numbers.
  </p>
</article>

<article class="project" id="ml-aero">
  <h3>Machine-learning surrogates for aerodynamic prediction</h3>
  <p class="meta">
    <b>IIT Madras Summer Fellowship</b> &middot; May &ndash; Jul 2024<br>
    CNN / ANN / PINN &middot; PyTorch + CUDA &middot; XFoil-generated training data
  </p>
  <p>
    A focused look at where learning can shortcut classical aerodynamics: I trained a
    convolutional network on XFoil-generated data to predict lift and drag coefficients
    directly from airfoil images, alongside ANN and physics-informed baselines. The
    result was a working proof of concept for ML-accelerated aerodynamic prediction
    &mdash; and a useful counterpoint to the first-principles simulation work I do now.
  </p>
</article>
