---
title: "PURExpress Cytosol Assembly with Broccoli 2/mScarlet Reporter"
description: |
  A standard PURExpress cell-free protein synthesis reaction using a Broccoli 2 RNA aptamer and mScarlet reporter plasmid was assembled to test whether transcription and translation could be detected in real time by fluorescence in a defined reconstituted cytosol.
date: 2026-04-03
authors:
  - name: Lord Kelvinho
    email: antonmolina@bnext.bio
    affiliation: b.next
keywords:
  - cell-free protein synthesis
  - PURExpress
  - Broccoli aptamer
  - mScarlet
  - CFPS
  - cytosol assembly
license: CC-BY-4.0
thumbnail: kinetics-broccoli-mscarlet.png
collections:
  - REVIEW: inferred — nucleus-core, cal-poly
id: dn-2026-ccby-purexpress-broccoli-mscarlet
---

# Overview

This DevNote characterizes a standard PURExpress cell-free protein synthesis reaction using a Broccoli 2 RNA aptamer and mScarlet reporter plasmid. The goal was to test whether transcription and translation could be detected in real time by fluorescence in a defined reconstituted cytosol. The reaction used the CP/CK energy regeneration system built into standard PURExpress Solution A and included a no-DNA negative control to confirm that fluorescence depended on template-driven expression. This experiment follows the CHEM 471 Experiment 1 cytosol assembly workflow and supports later synthetic-cell work where cytosol performance is tested inside membrane compartments.

# Methods

## Reaction composition

:::{table} PURExpress reaction composition for Broccoli 2/mScarlet expression
:label: tbl-reaction-composition
:align: center

| Component | Input concentration | Unit | Final concentration | Unit | Volume (µL) |
| --- | --- | --- | --- | --- | --- |
| PURExpress Solution A | — | — | — | — | 8.0 |
| PURExpress Solution B | — | — | — | — | 6.0 |
| RNase inhibitor | — | — | — | — | 0.5 |
| DNA template: Broccoli 2 mScarlet | 48.4 | ng/µL | ~5 | ng/µL | 2.1 |
| DFHBI | — | — | — | — | 2.0 |
| Nuclease-free H2O | — | — | — | — | 1.43 |
| Total | | | | | 20.0 |

Two positive reactions (+PURE Rep 1 and +PURE Rep 2) were assembled using the volumes above. The no-DNA negative control replaced the 2.1 µL DNA template with an additional 2.1 µL nuclease-free H2O (total H2O = 3.5 µL) and omitted DNA template.
:::

## Assembly

1. Retrieved PURExpress Solution A and Solution B from -20 °C storage and thawed both on ice for 5–10 minutes.
2. Kept all components on ice during reaction assembly. Solution B was handled gently because it contains ribosomes and should not be vortexed.
3. Labeled reaction tubes for two positive +PURE reactions and one no-DNA negative control.
4. Added Solution A, Solution B, RNase inhibitor, DNA template where applicable, nuclease-free water, and DFHBI according to the reaction composition table ({ref}`tbl-reaction-composition`).
5. Mixed each reaction gently by pipetting up and down 10–15 times until homogeneous and clear.
6. Briefly spun tubes in a minicentrifuge to collect liquid and remove bubbles, then held assembled reactions on ice before plating.

## Plating and plate reader setup

1. Transferred reactions to a black 384-well optical plate according to the assigned plate map.
2. Used technical duplicate wells for positive reactions when possible and included the no-DNA control.
3. Measured fluorescence kinetics for approximately 4 hours. Plate reader settings: excitation 485 nm, emission 528 nm, 30 °C, reads every 5–10 minutes.

# Results

Fluorescence was tracked over 4 hours for both the RNA aptamer signal and mScarlet protein production. The plotted data showed increasing fluorescence in the positive reactions, while the no-DNA controls remained close to baseline. This supports successful transcription and translation in the PURExpress reaction and confirms that the observed signal was template-dependent.

:::{figure} kinetics-broccoli-mscarlet.png
:label: fig-broccoli-mscarlet-kinetics
:align: center
:width: 75%
Broccoli 2 (48.4 ng/µL) and mScarlet fluorescence kinetics in a PURExpress CFPS reaction. Broccoli fluorescence was monitored as a readout of RNA aptamer transcription, while mScarlet fluorescence was monitored as a readout of protein production.
:::

REVIEW: source figure was embedded in Word doc as media/image1.png — confirm kinetics-broccoli-mscarlet.png is the extracted and renamed version of this file.

# Conclusions

These results demonstrate that transcription and translation can be detected in real time using a Broccoli 2/mScarlet dual reporter in a PURExpress cell-free system. The no-DNA negative control confirmed that the observed fluorescence signal was template-dependent. This cytosol assembly protocol provides a baseline characterization for subsequent experiments testing cytosol performance inside membrane compartments.

# References

- CHEM 471 Engineering Synthetic Cells Laboratory Manual, Experiment 1 — Cytosol Assembly.