---
title: "PURExpress Cytosol Assembly with Broccoli 2/mScarlet Reporter"
description: |
  A standard PURExpress cell-free protein synthesis reaction using a Broccoli 2 RNA aptamer and mScarlet reporter plasmid was assembled to test whether transcription and translation could be detected in real time by fluorescence in a defined reconstituted cytosol.
date: 2026-04-03
authors:
  - name: Sir Newton
    affiliation: b.next
    email: antonmolina@bnext.bio
keywords:
  - cell-free protein synthesis
  - PURExpress
  - Broccoli aptamer
  - mScarlet
  - cytosol assembly
  - CFPS
license: CC-BY-4.0
thumbnail: kinetics-broccoli-mscarlet.png
collections:
  - REVIEW: inferred — nucleus-core, cal-poly
id: dn-2026-ccby-purexpress-cytosol-broccoli-mscarlet
---

# Overview

This DevNote characterizes a standard PURExpress cell-free protein synthesis reaction using a Broccoli 2 RNA aptamer and mScarlet reporter plasmid. The goal was to test whether transcription and translation could be detected in real time by fluorescence in a defined reconstituted cytosol. The reaction used the CP/CK energy regeneration system built into standard PURExpress Solution A and included a no-DNA negative control to confirm that fluorescence depended on template-driven expression. This experiment follows the CHEM 471 Experiment 1 cytosol assembly workflow and supports later synthetic-cell work where cytosol performance is tested inside membrane compartments.

# Methods

## Reaction composition

:::{table} PURExpress CFPS reaction composition for Broccoli 2/mScarlet expression
:label: tbl-reaction-composition
:align: center

| Component | Input concentration | Unit | Final concentration | Unit | Volume (µL) |
| --- | --- | --- | --- | --- | --- |
| PURExpress Solution A | — | — | — | — | 8.0 |
| PURExpress Solution B | — | — | — | — | 6.0 |
| RNase inhibitor | — | — | — | — | 0.5 |
| DNA template: Broccoli 2 mScarlet | 48.4 | ng/µL | ~5 | ng/µL | 2.1 |
| Nuclease-free H2O | — | — | — | — | 1.43 |
| DFHBI | — | — | — | — | 2.0 |
| Total | | | | | 20.0 |

The no-DNA negative control substituted 3.5 µL nuclease-free H2O in place of the 2.1 µL DNA template and 1.43 µL nuclease-free H2O used in the positive reactions.
:::

## Assembly

1. Retrieved PURExpress Solution A and Solution B from -20 °C storage and thawed both on ice for 5–10 minutes.
2. Kept all components on ice during reaction assembly. Solution B was handled gently because it contains ribosomes and should not be vortexed.
3. Labeled reaction tubes for two positive +PURE reactions and one no-DNA negative control.
4. Added Solution A, Solution B, RNase inhibitor, DNA template where applicable, nuclease-free water, and DFHBI according to the reaction composition table.
5. Mixed each reaction gently by pipetting up and down 10–15 times until homogeneous and clear.
6. Briefly spun tubes in a minicentrifuge to collect liquid and remove bubbles, then held assembled reactions on ice before plating.

## Plating and plate reader setup

1. Transferred reactions to a black 384-well optical plate according to the assigned plate map.
2. Used technical duplicate wells for positive reactions when possible and included the no-DNA control.
3. Measured fluorescence kinetics for approximately 4 hours. Plate reader settings: excitation 485 nm, emission 528 nm, 30 °C, reads every 5–10 minutes.

# Results

Fluorescence was tracked over 4 hours for both the RNA aptamer signal and mScarlet protein production. The plotted data showed increasing fluorescence in the positive reactions, while the no-DNA controls remained close to baseline. This supports successful transcription and translation in the PURExpress reaction and confirms that the observed signal was template-dependent.

:::{figure} kinetics-broccoli-mscarlet.png
:label: fig-kinetics-broccoli-mscarlet
:align: center
:width: 75%
Broccoli 2 (48.4 ng/µL) and mScarlet fluorescence kinetics in a PURExpress CFPS reaction. Broccoli fluorescence was monitored as a readout of RNA aptamer transcription, while mScarlet fluorescence was monitored as a readout of protein production.
:::

# Conclusions

A PURExpress cell-free protein synthesis reaction using a Broccoli 2/mScarlet reporter plasmid produced template-dependent fluorescence signal over a 4-hour timecourse, confirming that transcription and translation were active under the assembled conditions. The no-DNA negative control remained near baseline, establishing that the observed fluorescence was not a result of reagent autofluorescence or contamination. This cytosol assembly protocol supports downstream experiments in which cell-free reactions are encapsulated inside membrane compartments.

# References

- CHEM 471 Engineering Synthetic Cells Laboratory Manual, Experiment 1 — Cytosol Assembly.