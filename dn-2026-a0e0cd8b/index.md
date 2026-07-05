---
title: "PURExpress Cytosol Assembly with Broccoli 2/mScarlet Reporter"
description: |
  A standard PURExpress cell-free protein synthesis reaction using a Broccoli 2 RNA aptamer and mScarlet reporter plasmid was assembled and monitored by fluorescence kinetics over 4 hours, confirming template-dependent transcription and translation in a defined reconstituted cytosol.
date: 2026-04-03
authors:
  - name: adam smith
    affiliation: b.next
    email: build@bnext.bio
keywords:
  - cell-free protein synthesis
  - PURExpress
  - Broccoli 2
  - mScarlet
  - RNA aptamer
  - cytosol assembly
license: CC-BY-4.0
thumbnail: kinetics-broccoli-mscarlet.png
collections:
  - REVIEW: inferred — nucleus-core, cal-poly
id: dn-2026-a0e0cd8b
---

# Overview

This DevNote characterizes a standard PURExpress cell-free protein synthesis reaction using a Broccoli 2 RNA aptamer and mScarlet reporter plasmid. The goal was to test whether transcription and translation could be detected in real time by fluorescence in a defined reconstituted cytosol. The reaction used the CP/CK energy regeneration system built into standard PURExpress Solution A and included a no-DNA negative control to confirm that fluorescence depended on template-driven expression. This experiment follows the CHEM 471 Experiment 1 cytosol assembly workflow and supports later synthetic-cell work where cytosol performance is tested inside membrane compartments.

# Methods

## Reagents

:::{table} Bill of materials
:label: tbl-bom
:align: center

| Reagent | Product Name | Manufacturer | Storage Conditions |
| --- | --- | --- | --- |
| PURExpress Solution A | PURExpress Solution A with CP/CK energy system | New England Biolabs | −20 °C; thaw and hold on ice |
| PURExpress Solution B | PURExpress ribosome solution | New England Biolabs | −20 °C; thaw and hold on ice; do not vortex |
| RNase inhibitor | RNase inhibitor | — | — |
| DNA template | Broccoli 2 mScarlet DNA template, 48.4 ng/µL | — | — |
| DFHBI | Fluorogen for Broccoli aptamer | — | — |
| Nuclease-free H2O | Nuclease-free water | — | — |
| 384-well plate | Black optical 384-well plate | — | — |

:::

REVIEW: Catalog numbers, prices, and links were not provided in the source materials. Fill in before publishing.

## Reaction composition

:::{table} Reaction setup for PURExpress Broccoli 2/mScarlet CFPS
:label: tbl-reaction
:align: center

| Component | Input concentration | Unit | Final concentration | Unit | +PURE Rep 1 (µL) | +PURE Rep 2 (µL) | −PURE Control (µL) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Solution A | — | — | — | — | 8.0 | 8.0 | 8.0 |
| Solution B | — | — | — | — | 6.0 | 6.0 | 6.0 |
| RNase inhibitor | — | — | — | — | 0.5 | 0.5 | 0.5 |
| DNA template: Broccoli 2 mScarlet | 48.4 | ng/µL | ~5 | ng/µL | 2.1 | 2.1 | 0 |
| Nuclease-free H2O | — | — | — | — | 1.43 | 1.43 | 3.5 |
| DFHBI | — | — | — | — | 2.0 | 2.0 | 2.0 |
| Total | | | | | 20 | 20 | 20 |

:::

REVIEW: Stock concentrations for PURExpress Solution A and Solution B are proprietary and not available from the source. Record as — or confirm with NEB documentation before publishing.

## Assembly

1. Retrieved PURExpress Solution A and Solution B from −20 °C storage and thawed both on ice for 5–10 minutes.
2. Kept all components on ice during reaction assembly. Solution B was handled gently because it contains ribosomes and should not be vortexed.
3. Labeled reaction tubes for two positive +PURE reactions and one no-DNA negative control.
4. Added Solution A, Solution B, RNase inhibitor, DNA template where applicable, nuclease-free water, and DFHBI according to the reaction setup table ({ref}`tbl-reaction`).
5. Mixed each reaction gently by pipetting up and down 10–15 times until homogeneous and clear.
6. Briefly spun tubes in a minicentrifuge to collect liquid and remove bubbles, then held assembled reactions on ice before plating.

## Plating and plate reader setup

1. Transferred reactions to a black 384-well optical plate according to the assigned plate map.
2. Used technical duplicate wells for positive reactions when possible and included the no-DNA control.
3. Measured fluorescence kinetics for approximately 4 hours. Plate reader settings: excitation 485 nm, emission 528 nm, 30 °C, reads every 5–10 minutes.

# Results

Fluorescence was tracked over 4 hours for both the RNA aptamer signal and mScarlet protein production. The plotted data showed increasing fluorescence in the positive reactions, while the no-DNA controls remained close to baseline. This supports successful transcription and translation in the PURExpress reaction and confirms that the observed signal was template-dependent.

:::{figure} kinetics-broccoli-mscarlet.png
:label: fig-kinetics
:align: center
:width: 75%
Broccoli 2 (48.4 ng/µL) and mScarlet fluorescence kinetics in a PURExpress CFPS reaction. Broccoli fluorescence was monitored as a readout of RNA aptamer transcription, while mScarlet fluorescence was monitored as a readout of protein production.
:::

REVIEW: Source figure was embedded in Word doc as `media/image1.png`. Confirm that `figures/kinetics-broccoli-mscarlet.png` is the correct extracted file. If the pre-committed output `kinetics-broccoli-mscarlet.png` from the file inventory is the same figure, use that path directly.

# Conclusions and next steps

A PURExpress cell-free protein synthesis reaction expressing Broccoli 2 RNA aptamer and mScarlet protein was successfully assembled and monitored by fluorescence kinetics, with template-dependent signal confirmed by a no-DNA negative control. These findings establish a baseline cytosol performance benchmark for the Broccoli 2/mScarlet dual reporter system. Future work will test this cytosol formulation inside membrane compartments as part of the synthetic-cell assembly workflow.

# References

- CHEM 471 Engineering Synthetic Cells Laboratory Manual, Experiment 1 — Cytosol Assembly.