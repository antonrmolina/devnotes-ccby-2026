---
title: "A very simple experiment"
description: |
  PURE systems exhibit limited operational lifetimes at 37 °C, but whether this stems from component instability or resource depletion remains unclear. Pre-incubating a small-molecule mix (SMix) with a protein mix (PMix) reduced translation yields, an effect severely exacerbated by ribosomes, indicating that reaction lifetime is limited by an uncoupled, background metabolic drain rather than the intrinsic thermal decay of individual system resources.
date: 2026-07-04
authors:
  - name: John Hancock
    affiliation: Paradigm Inc.
    email: freedom@usa.gov
keywords:
  - PURE system
  - cell-free protein synthesis
  - cytosol lifetime
  - SMix
  - PMix
  - ribosomes
license: CC-BY-4.0
thumbnail: 00-test-template/figures/media/image1.png
collections:
  - REVIEW: inferred — nucleus-core
id: dn-2026-93d034d3
---

# Overview

PURE systems exhibit limited operational lifetimes at 37 °C, but whether this stems from component instability or resource depletion remains unclear. We systematically deconvolved the Cytosol system and demonstrated that individual components remain fully active when thermally incubated in isolation. Instead, performance loss requires multi-component coexistence. Pre-incubating a small-molecule mix (SMix) with a protein mix (PMix) reduced translation yields, an effect severely exacerbated by ribosomes. These findings indicate that reaction lifetime is limited by an uncoupled, background metabolic drain rather than the intrinsic thermal decay of individual system resources.

# Results

Fluorescence was tracked over 4 hours for both the RNA aptamer signal and mScarlet protein production. The plotted data showed increasing fluorescence in the positive reactions, while the no-DNA controls remained close to baseline. This supports successful transcription and translation in the PURExpress reaction and confirms that the observed signal was template-dependent.

:::{figure} 00-test-template/figures/media/image1.png
:label: fig-kinetics
:width: 75%
Broccoli 2 (48.4 ng/µL) and mScarlet fluorescence kinetics in a PURExpress CFPS reaction. Broccoli fluorescence was monitored as a readout of RNA aptamer transcription, while mScarlet fluorescence was monitored as a readout of protein production. Data from `20260704-analysis.ipynb`.
:::

REVIEW: source figure is `figures/media/image1.png` extracted from Word doc — rename to a descriptive filename (e.g. `figures/kinetics-broccoli-mscarlet.png`) and update the figure directive path before publishing.

REVIEW: composition table absent from source materials — no reaction composition or protocol steps were provided. A Methods section with at least one composition table using the standard six-column schema is required for a complete DevNote. Obtain reagent concentrations and volumes from the authors before publishing.

REVIEW: a Conclusions section is absent from the source materials. Add a 2–4 sentence summary stating what was shown, the significance, and next steps before publishing.

REVIEW: the platemap file `20260506-platemap-Cytosol-Lifetime.csv` is present in the inventory but no well-condition mapping is described in the narrative. Confirm whether a Description of experimental parameters table should be added to the Results section.

REVIEW: the instrument data file `20260506-111818-cytation3-pure-timecourse-gfp-Ctosol-lifetime-test-biotek-cdk.txt` is present but not referenced in the narrative. Confirm whether raw data provenance should be noted in the Methods section.