---
title: "A very simple experiment"
description: |
  PURE systems exhibit limited operational lifetimes at 37 °C, but whether this stems from component instability or resource depletion remains unclear. Pre-incubating a small-molecule mix (SMix) with a protein mix (PMix) reduced translation yields, an effect severely exacerbated by ribosomes, indicating that reaction lifetime is limited by an uncoupled, background metabolic drain rather than the intrinsic thermal decay of individual system resources.
date: 2026-07-04
authors:
  - name: fake fakerson
    affiliation: US Lan
    email: fake@gov.bio
keywords:
  - PURE system
  - cell-free protein synthesis
  - cytosol lifetime
  - component stability
  - resource depletion
license: CC-BY-4.0
thumbnail: 00-test-template/figures/media/image1.png
collections:
  - REVIEW: inferred — nucleus-core
id: dn-2026-a8c0096d
---

# Overview

PURE systems exhibit limited operational lifetimes at 37 °C, but whether this stems from component instability or resource depletion remains unclear. We systematically deconvolved the Cytosol system and demonstrated that individual components remain fully active when thermally incubated in isolation. Instead, performance loss requires multi-component coexistence. Pre-incubating a small-molecule mix (SMix) with a protein mix (PMix) reduced translation yields, an effect severely exacerbated by ribosomes. These findings indicate that reaction lifetime is limited by an uncoupled, background metabolic drain rather than the intrinsic thermal decay of individual system resources.

# Results and Observations

Fluorescence was tracked over 4 hours for both the RNA aptamer signal and mScarlet protein production. The plotted data showed increasing fluorescence in the positive reactions, while the no-DNA controls remained close to baseline. This supports successful transcription and translation in the PURExpress reaction and confirms that the observed signal was template-dependent.

:::{figure} 00-test-template/figures/media/image2.png
:label: fig-kinetics
:width: 75%
This data is from 20260704-analysis.ipynb. Broccoli 2 (48.4 ng/µL) and mScarlet fluorescence kinetics in a PURExpress CFPS reaction. Broccoli fluorescence was monitored as a readout of RNA aptamer transcription, while mScarlet fluorescence was monitored as a readout of protein production.
:::

This is a totally new observation

:::{figure} 00-test-template/figures/media/image1.png
:label: fig-crazy
:width: 75%
This is a crazy figure from 20260704-analysis.ipynb.
:::