---
layout: archive
title: "Portfolio"
permalink: /portfolio/
author_profile: true
redirect_from:
  - /software/
---

<p class="lede">Software built around a simple idea: the hard part of computational materials science should be the science. The research code lives in <a href="https://github.com/seixas-research">seixas-research</a>, applied data science and ML engineering in <a href="https://github.com/seixas-solutions">seixas-solutions</a>, teaching material in <a href="https://github.com/seixas-teaching">seixas-teaching</a>, and everything built for the joy of it in <a href="https://github.com/seixas-fun">seixas-fun</a>.</p>

## Featured products

<div class="card-grid">
  <div class="card">
    <h3 class="card__title"><a href="https://poraque.seixas.dev">Poraquê</a></h3>
    <p class="card__tagline">Machine learning density-based operators.</p>
    <div class="card__body">
      <p>Poraquê is a software framework for machine learning operators between the real-space fields of density functional theory. Given only a crystal geometry, it predicts the charge density and the kinetic energy density. No wavefunctions, no self-consistency cycle.</p>
      <ul>
        <li>Two Fourier Neural Operators: the Hohenberg–Kohn map, and the kinetic energy density functional missing from orbital-free DFT</li>
        <li>Density-based operators as first-class objects</li>
        <li>Built for the standard scientific Python stack (PyTorch, ASE)</li>
      </ul>
    </div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">PyTorch</span><span class="pill">In development</span></div>
    <div class="card__links"><a href="https://poraque.seixas.dev">Website</a><a href="https://poraque.readthedocs.io/">Manual</a><a href="https://pypi.org/project/poraque/">PyPI</a><a href="https://github.com/seixas-research/poraque">Source</a></div>
  </div>

  <div class="card">
    <h3 class="card__title"><a href="https://calango.seixas.dev">Calango</a></h3>
    <p class="card__tagline">Visual atomistic modeling.</p>
    <div class="card__body">
      <p>A desktop application that brings three things into one window: an interactive viewer for building, editing and inspecting atomic structures; a calculator-agnostic environment for setting up and running simulations; and viewers that turn the output back into figures you can read.</p>
      <ul>
        <li>Builders for slabs, interfaces, dislocations, polycrystals, nanotubes, nanoribbons and special quasirandom structures</li>
        <li>Materials Project, PubChem and C2DB one search away</li>
        <li>Written in C++20 with Qt 6, responsive at tens of thousands of atoms</li>
      </ul>
    </div>
    <div class="card__meta"><span class="pill">C++</span><span class="pill">Qt 6</span><span class="pill">In development</span></div>
    <div class="card__links"><a href="https://calango.seixas.dev">Website</a><a href="https://calango.readthedocs.io/">Manual</a><a href="https://github.com/seixas-research/calango">Source</a></div>
  </div>

  <div class="card">
    <h3 class="card__title"><a href="https://carcara.seixas.dev">Carcará</a></h3>
    <p class="card__tagline">Fermionic quantum simulation, one API.</p>
    <div class="card__body">
      <p>A lightweight Python framework for fermionic quantum simulation based on variational quantum algorithms. From a molecular or periodic geometry, it builds real-space grids, evaluates the one- and two-body integrals, maps the Hamiltonian to qubits, and solves it variationally — through a single ASE calculator that runs unchanged on IBM Qiskit, Amazon Braket and Google Cirq.</p>
      <ul>
        <li>VQE, ADAPT-VQE, excited states and a stochastic solver (VASQE), sharing one driver</li>
        <li>Localized basis sets and pseudopotentials generated from scratch, not tabulated</li>
        <li>Cross-backend agreement to 1.3×10⁻⁷ Ha, validated on real quantum hardware</li>
      </ul>
    </div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">Quantum computing</span><span class="pill">In development</span></div>
    <div class="card__links"><a href="https://carcara.seixas.dev">Website</a><a href="https://carcara.readthedocs.io/">Manual</a><a href="https://pypi.org/project/carcara/">PyPI</a><a href="https://github.com/seixas-research/carcara">Source</a></div>
  </div>
</div>

## Research tools

Smaller packages that come out of the research directly, published on PyPI under [seixas-research](https://github.com/seixas-research).

<div class="card-grid">
  <div class="card">
    <h3 class="card__title"><a href="https://oncapintada.readthedocs.io">Onça-pintada</a></h3>
    <p class="card__tagline">Thermodynamics of alloys.</p>
    <div class="card__body">Computes enthalpy, entropy and Gibbs free energy of mixing for binary and multicomponent alloys within the subregular solution model, together with binodal and spinodal curves. Cluster interactions are evaluated in the quasi-chemical approximation, which lets it describe chemical short-range order and rebuild atomistic geometries from short-range order metrics.</div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">Alloys</span><span class="pill">Thermodynamics</span></div>
    <div class="card__links"><a href="https://oncapintada.readthedocs.io">Manual</a><a href="https://pypi.org/project/oncapintada/">PyPI</a><a href="https://github.com/seixas-research/oncapintada">Source</a></div>
  </div>

  <div class="card">
    <h3 class="card__title"><a href="https://github.com/seixas-research/sagui">SAGUI</a></h3>
    <p class="card__tagline">Machine-learned interatomic potentials and generative models.</p>
    <div class="card__body">Scalable Atomistic Graph networks for Universal Interactions: an equivariant graph neural network framework that learns energies and forces from the same structures it learns the distribution of structures from. Two interchangeable architectures — a many-body ACE-style message-passing model and a strictly local one — with the O(3) tensor algebra implemented from scratch, no <code>e3nn</code> dependency.</div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">PyTorch</span><span class="pill">MLIP</span><span class="pill">In development</span></div>
    <div class="card__links"><a href="https://github.com/seixas-research/sagui">Source</a></div>
  </div>

  <div class="card">
    <h3 class="card__title"><a href="https://pypi.org/project/blendpy/">Blendpy</a></h3>
    <p class="card__tagline">Alloy thermodynamics from first principles.</p>
    <div class="card__body">A toolkit for investigating thermodynamic models of alloys with first-principles calculations: enthalpy of mixing and the spinodal and binodal decomposition curves of a phase diagram, through the dilute solution interpolation model, driven by any ASE calculator.</div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">ASE</span><span class="pill">Phase diagrams</span></div>
    <div class="card__links"><a href="https://pypi.org/project/blendpy/">PyPI</a><a href="https://github.com/seixas-research/blendpy">Source</a></div>
  </div>

  <div class="card">
    <h3 class="card__title"><a href="https://doi.org/10.5281/zenodo.14963121">Quasigraph</a></h3>
    <p class="card__tagline">Descriptors for materials machine learning.</p>
    <div class="card__body">A graph-like chemical and geometric descriptor toolkit: from an ASE <code>Atoms</code> object it produces a dataframe or a vector combining a chemical part and a coordination-number-based geometric part, ready to feed a machine learning model.</div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">Descriptors</span><span class="pill">Materials informatics</span></div>
    <div class="card__links"><a href="https://doi.org/10.5281/zenodo.14963121">DOI</a><a href="https://pypi.org/project/quasigraph/">PyPI</a><a href="https://github.com/seixas-research/quasigraph">Source</a></div>
  </div>

  <div class="card">
    <h3 class="card__title"><a href="https://github.com/seixas-research/calango-cli">calango-cli</a></h3>
    <p class="card__tagline">Calango workflows, headless.</p>
    <div class="card__body">Runs a pipeline built on the Calango orchestration canvas without a display: export the workflow to a single self-contained JSON document, copy it to an HPC cluster, run it there, and load the results straight back into the GUI.</div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">HPC</span></div>
    <div class="card__links"><a href="https://github.com/seixas-research/calango-cli">Source</a></div>
  </div>
</div>

## Data science &amp; ML engineering

Applied work under [seixas-solutions](https://github.com/seixas-solutions).

<div class="card-grid">
  <div class="card">
    <h3 class="card__title"><a href="https://github.com/seixas-solutions/sucuri">Sucuri</a></h3>
    <p class="card__tagline">Anomaly signals in Brazilian federal spending on higher education.</p>
    <div class="card__body">Collects, cleans and analyses budget execution from the Ministry of Education through the Portal da Transparência API — federal universities, institutes, university hospitals, CAPES, FNDE/FIES — enriched with contracts, procurement, sanctions and IBGE population and GDP data. It flags statistically atypical spending patterns worth a manual check; statistical atypicality is not evidence of irregularity.</div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">Open data</span><span class="pill">Anomaly detection</span></div>
    <div class="card__links"><a href="https://github.com/seixas-solutions/sucuri">Source</a></div>
  </div>

  <div class="card">
    <h3 class="card__title"><a href="https://github.com/seixas-solutions/papagaio">Papagaio</a></h3>
    <p class="card__tagline">Local-first AI speech refinement for Apple Silicon.</p>
    <div class="card__body">Transcribes spoken audio with word-level timestamps, detects filler words, stutters, repetitions, dead air and rushed delivery, and renders a cleaned-up version that still sounds like the same person in the same room. Everything runs on the machine, with MLX — no uploads, no API keys.</div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">MLX</span><span class="pill">Whisper</span><span class="pill">Alpha</span></div>
    <div class="card__links"><a href="https://github.com/seixas-solutions/papagaio">Source</a></div>
  </div>
</div>

## For fun

<div class="card-grid">
  <div class="card">
    <h3 class="card__title"><a href="https://tamandua.games">Tamanduá</a></h3>
    <p class="card__tagline">Can you guess all the flags?</p>
    <div class="card__body">A flag-guessing game across national flags, 2026 World Cup teams and the 26 Brazilian states plus the Federal District, in multiple-choice or type-the-name mode.</div>
    <div class="card__meta"><span class="pill">Python</span><span class="pill">Web app</span></div>
    <div class="card__links"><a href="https://tamandua.games">Play</a><a href="https://github.com/seixas-fun/tamandua">Source</a></div>
  </div>
</div>

## Teaching material

Notebooks and tutorials used in courses are published in [seixas-teaching](https://github.com/seixas-teaching) and listed on the [CV](/cv/#teaching).

---

Have a problem worth computing? I am open to research collaborations and consulting on scientific software and applied machine learning — [start a conversation](/contact/).
