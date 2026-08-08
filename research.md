---
title: Research
eyebrow: Research
subtitle: High-fidelity simulation of compressible flows — where fast-moving waves meet the things they run into, and the numerics that make both tractable.
permalink: /research/
---

<article class="project" id="phd-shock">
  <h3>Shock wave interaction with structures and materials <span class="tag">Ongoing</span></h3>
  <p class="meta">
    <b>PhD, IIT Bombay</b> &middot; Department of Aerospace Engineering &middot; Jul 2026 &ndash; present
  </p>
  <p>
    My doctoral work sits at the coupling between a compressible flow and the
    solid it loads: what a shock does to a structure or material as it arrives,
    reflects, and diffracts, and how the deforming boundary feeds back into the
    wave field. It is a two-way problem &mdash; the flow sets the loading, the
    structure changes the flow &mdash; and resolving it faithfully means carrying
    the shock, the interface, and the material response in the same picture. This
    is the direction the rest of my work below was quietly building toward:
    from incompressible wakes, to compressible two-phase flow, to fast flows that
    push on things.
  </p>
</article>

<article class="project" id="dns-cylinder">
  <h3>DNS of compressible gas&ndash;droplet flow past a circular cylinder</h3>
  <p class="meta">
    <b>IIT Madras</b>, with Prof. A. Sameen &middot; Dec 2024 &ndash; Jul 2026<br>
    Re = 100, Ma = 0.1 &middot; six-equation two-fluid model &middot; ~8,100-line Fortran&nbsp;90 unstructured finite-volume solver &middot; HLLC &middot; eSSPRK(4,3) &middot; METIS/MPI &middot; OpenACC GPU offload
  </p>
  <p>
    The core of my time at IIT Madras: resolving the wake of a circular cylinder
    in a compressible gas&ndash;droplet flow with an in-house Fortran&nbsp;90
    unstructured finite-volume solver &mdash; HLLC Riemann fluxes, an eSSPRK(4,3)
    time march, METIS/MPI domain decomposition, and OpenACC offload. Beyond
    running the physics, much of the work was making the solver fast and correct
    on GPUs:
  </p>
  <ul>
    <li>Re-engineered the code for GPU throughput &mdash; replaced whole-array PCIe transfers and per-variable blocking <code>Sendrecv</code> with GPU-side pack/unpack into persistent flat buffers and a single nonblocking <code>Isend</code>/<code>Irecv</code> pair per neighbour. Roughly <b>11&times; end-to-end speedup</b> on a 20,000-iteration production run, with the core time-march output bit-identical to the original.</li>
    <li>Diagnosed and fixed a GPU data race in the residual reduction that had made convergence residuals nondeterministic, and a launch defect binding every MPI rank to GPU&nbsp;0 instead of one GPU per rank.</li>
    <li>Traced spurious near-wall flow and unphysical spanwise structures to a blocking defect in the ICEM O-grids; rebuilt the mesh pipeline in GMSH and qualified a clean 3.5M-cell tetrahedral case, with meshes up to 28M cells evaluated.</li>
    <li>Corrected a pressure-reflecting outlet and an overspecified inlet that were trapping outgoing acoustic waves inside the domain.</li>
    <li>Validated shedding frequency against published Strouhal-number data and quantified droplet-loading effects on the wake.</li>
  </ul>
  <p class="meta">
    Production runs under SLURM on NVIDIA A100 nodes (hoopoe) and on PARAM Shakti (C-DAC NSM); multi-rank unstructured post-processing in Tecplot&nbsp;360 / PyTecplot and ParaView.
  </p>
</article>

<article class="project" id="thesis-solver">
  <h3>A compressible multifluid solver for gas&ndash;liquid flow past a bluff body</h3>
  <p class="meta">
    <b>B.Tech thesis</b> &middot; Dec 2024 &ndash; Jun 2025 &middot; carried out at IIT Madras (host: Prof. A. Sameen); thesis guide: Dr. Aldin Justin Sundaraj, KITS<br>
    Six-equation two-fluid model &middot; HLLC &middot; unstructured finite volume
  </p>
  <p>
    My undergraduate thesis laid the groundwork the DNS effort stands on: a
    three-dimensional finite-volume solver for compressible gas&ndash;liquid
    two-phase flow using a six-equation two-fluid model. I validated it against
    the air&ndash;water shock-tube benchmark &mdash; recovering shock propagation,
    the expansion fan, and the material interface &mdash; and against published
    Strouhal data for single-phase cylinder flow. Quantifying droplet loading, the
    Strouhal number fell from 0.221 (single phase) to 0.211 at 0.1% dispersed
    volume fraction, consistent with interfacial drag damping the vortex roll-up.
  </p>
</article>

<article class="project" id="ml-aero">
  <h3>Machine-learning surrogates for aerodynamic prediction</h3>
  <p class="meta">
    <b>IIT Madras Summer Fellowship</b> &middot; May &ndash; Jul 2024<br>
    ANN / CNN / PINN &middot; PyTorch + CUDA &middot; XFoil-generated training data
  </p>
  <p>
    A focused look at where learning can shortcut classical aerodynamics: I trained
    a convolutional network on XFoil-generated data to predict lift and drag
    coefficients directly from airfoil images, alongside ANN and physics-informed
    baselines. The result was a working proof of concept for ML-accelerated
    aerodynamic prediction &mdash; and a useful counterpoint to the first-principles
    simulation that has occupied me since.
  </p>
</article>
