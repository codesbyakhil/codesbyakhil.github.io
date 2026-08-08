---
title: Experience
eyebrow: Experience & Education
subtitle: Roles, training, and the toolset built along the way.
permalink: /experience/
---

<div class="role">
  <span class="when">Jul 2026 &ndash;<br>present</span>
  <div>
    <h3>PhD Scholar</h3>
    <p class="where">Department of Aerospace Engineering, IIT Bombay</p>
    <ul>
      <li>Doctoral research on shock wave interaction with structures and materials &mdash; wave loading, reflection and diffraction, and the two-way coupling between a compressible flow and the solid it acts on.</li>
    </ul>
  </div>
</div>

<div class="role">
  <span class="when">Jul 2025 &ndash;<br>Jul 2026</span>
  <div>
    <h3>Project Associate</h3>
    <p class="where">Department of Aerospace Engineering, IIT Madras &mdash; Prof. A. Sameen's group</p>
    <ul>
      <li>Six-equation two-fluid DNS of compressible gas&ndash;droplet flow past a circular cylinder (Re = 100, Ma = 0.1) with an in-house ~8,100-line Fortran&nbsp;90 unstructured finite-volume solver (HLLC, eSSPRK(4,3), METIS/MPI, OpenACC GPU offload).</li>
      <li>Re-engineered the MPI halo exchange for GPUs &mdash; GPU-side pack/unpack into persistent flat buffers, one nonblocking <code>Isend</code>/<code>Irecv</code> pair per neighbour &mdash; for a ~11&times; end-to-end speedup, output bit-identical to the original code.</li>
      <li>Fixed a GPU data race in the residual reduction and a launch defect binding every rank to GPU&nbsp;0 instead of one GPU per rank.</li>
      <li>Rebuilt a defective ICEM O-grid mesh pipeline in GMSH; qualified a clean 3.5M-cell tetrahedral case, with meshes up to 28M cells evaluated.</li>
      <li>Corrected pressure-reflecting outlet and overspecified inlet conditions that trapped outgoing acoustic waves in the domain.</li>
      <li>Validated shedding frequency against Strouhal data; ran production jobs under SLURM on A100 nodes and PARAM Shakti; post-processed in Tecplot&nbsp;360 / PyTecplot and ParaView.</li>
    </ul>
  </div>
</div>

<div class="role">
  <span class="when">Dec 2024 &ndash;<br>Jun 2025</span>
  <div>
    <h3>Research Intern</h3>
    <p class="where">Department of Aerospace Engineering, IIT Madras</p>
    <ul>
      <li>Set up compressible multiphase simulations with a six-equation two-fluid model in an in-house Fortran&nbsp;90 finite-volume code &mdash; the work that became my B.Tech thesis.</li>
      <li>Applied DNS to laminar vortex shedding and gas&ndash;droplet interface dynamics around a cylinder at low Reynolds numbers (Re = 100 and 150, Ma = 0.1).</li>
      <li>Validated against the air&ndash;water shock-tube benchmark (shock propagation, expansion waves, material interface) and published Strouhal data; quantified droplet-loading effects on shedding.</li>
    </ul>
  </div>
</div>

<div class="role">
  <span class="when">May &ndash; Jul<br>2024</span>
  <div>
    <h3>Summer Fellow</h3>
    <p class="where">IIT Madras Summer Fellowship Programme</p>
    <ul>
      <li>Applied machine learning to aerodynamic prediction: ANN, CNN, and PINN models in PyTorch with CUDA.</li>
      <li>Trained a CNN on XFoil-generated data to predict lift and drag coefficients from airfoil images; delivered a proof of concept for ML-accelerated aerodynamics.</li>
    </ul>
  </div>
</div>

<div class="role">
  <span class="when">Jun 2023</span>
  <div>
    <h3>Internship Trainee</h3>
    <p class="where">Hindustan Aeronautics Limited, Bengaluru</p>
    <ul>
      <li>Hands-on exposure to the LCA Tejas production line: component fabrication, structural assembly, and system integration in a live defence-aviation environment.</li>
    </ul>
  </div>
</div>

<div class="role">
  <span class="when">2021 &ndash; 2022</span>
  <div>
    <h3>Earlier internships &amp; activities</h3>
    <p>
      Summer intern at Omspace Rocket &amp; Exploration (launch vehicles, 2022); internship
      trainee at Brahmastra Aerospace Systems (industrial aerodynamics, 2022; aircraft
      vehicle design, 2021&ndash;22); quantum-computing internship at XUANTA Developers
      (2022); student delegate at the 7th Bangalore Space Expo (CII, 2022). Media
      coordinator at Gravitace, KITS (2023&ndash;24). Student member of the Aeronautical
      Society of India (2023&ndash;26).
    </p>
  </div>
</div>

## Education

<div class="role">
  <span class="when">2026 &ndash;<br>present</span>
  <div>
    <h3>PhD, Aerospace Engineering</h3>
    <p class="where">Indian Institute of Technology Bombay</p>
    <p>Shock wave interaction with structures and materials.</p>
  </div>
</div>

<div class="role">
  <span class="when">2021 &ndash; 2025</span>
  <div>
    <h3>B.Tech, Aerospace Engineering</h3>
    <p class="where">Karunya Institute of Technology and Sciences, Coimbatore</p>
    <p>
      Thesis: <em>Numerical simulation of flow over a bluff body using a compressible
      multifluid six-equation formulation</em> &mdash; carried out at IIT Madras.
    </p>
  </div>
</div>

## Toolset

<ul class="tags">
  <li class="tag">Fortran 90</li>
  <li class="tag">MPI</li>
  <li class="tag">OpenACC</li>
  <li class="tag">GPU computing</li>
  <li class="tag">DNS</li>
  <li class="tag">Compressible flow</li>
  <li class="tag">Riemann solvers</li>
  <li class="tag">GMSH</li>
  <li class="tag">ICEM CFD</li>
  <li class="tag">ANSYS Fluent</li>
  <li class="tag">PyTorch</li>
  <li class="tag">Tecplot / ParaView</li>
  <li class="tag">SLURM</li>
  <li class="tag">CATIA</li>
  <li class="tag">LaTeX</li>
</ul>

<p class="pub-detail" style="margin-top:1.4rem">
  Languages: English (professional working) &middot; Malayalam and Hindi (native/bilingual) &middot; Tamil (limited working).
</p>
