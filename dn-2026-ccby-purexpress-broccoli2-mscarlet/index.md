---
title: "PURExpress Cytosol Assembly with Broccoli 2/mScarlet Reporter"
description: |
  A PURExpress cell-free protein synthesis reaction using a Broccoli 2 RNA aptamer and mScarlet reporter plasmid was assembled and monitored by fluorescence kinetics over 4 hours, confirming that transcription and translation could be detected in real time in a defined reconstituted cytosol.
date: 2026-04-03
authors:
  - name: Sam Cell
    affiliation: Cal Poly
    email: samcell@calpoly.edu
keywords:
  - cell-free protein synthesis
  - PURExpress
  - Broccoli aptamer
  - mScarlet
  - fluorescence kinetics
  - cytosol assembly
license: CC-BY-4.0
thumbnail: figures/kinetics-broccoli-mscarlet.png
collections:
  - REVIEW: inferred — nucleus-core, cal-poly
id: dn-2026-ccby-purexpress-broccoli2-mscarlet
---

# Overview

This DevNote characterizes a standard PURExpress cell-free protein synthesis reaction using a Broccoli 2 RNA aptamer and mScarlet reporter plasmid. The goal was to test whether transcription and translation could be detected in real time by fluorescence in a defined reconstituted cytosol. The reaction used the CP/CK energy regeneration system built into standard PURExpress Solution A and included a no-DNA negative control to confirm that fluorescence depended on template-driven expression. This experiment follows the CHEM 471 Experiment 1 cytosol assembly workflow and supports later synthetic-cell work where cytosol performance is tested inside membrane compartments.

# Methods

## Reagents

:::{table} Reagents used in this experiment.
:label: tbl-bom
:align: center

| Reagent | Description | Manufacturer | Storage |
| --- | --- | --- | --- |
| PURExpress Solution A | PURExpress Solution A with CP/CK energy system | New England Biolabs | −20 °C; thaw and hold on ice |
| PURExpress Solution B | PURExpress ribosome solution | New England Biolabs | −20 °C; thaw and hold on ice; do not vortex |
| RNase inhibitor | RNase inhibitor | — | REVIEW: storage conditions not provided |
| DNA template | Broccoli 2 mScarlet DNA template, 48.4 ng/µL | — | REVIEW: source and storage not provided |
| DFHBI | Fluorogen for Broccoli aptamer | — | REVIEW: supplier and storage not provided |
| Nuclease-free H₂O | Nuclease-free water | — | — |
| 384-well plate | Black optical 384-well plate | — | — |

:::

## Reaction composition

:::{table} Reaction composition for PURExpress CFPS reactions. Two positive replicates (+PURE Rep 1, +PURE Rep 2) and one no-DNA negative control (−PURE Control) were assembled at a total volume of 20 µL each.
:label: tbl-reaction
:align: center

| Component | Input concentration | Unit | Final concentration | Unit | +PURE Rep 1 (µL) | +PURE Rep 2 (µL) | −PURE Control (µL) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| PURExpress Solution A | — | — | — | — | 8.0 | 8.0 | 8.0 |
| PURExpress Solution B | — | — | — | — | 6.0 | 6.0 | 6.0 |
| RNase inhibitor | — | — | — | — | 0.5 | 0.5 | 0.5 |
| DNA template: Broccoli 2 mScarlet | 48.4 | ng/µL | ~5 | ng/µL | 2.1 | 2.1 | 0 |
| Nuclease-free H₂O | — | — | — | — | 1.43 | 1.43 | 3.5 |
| DFHBI | — | — | — | — | 2.0 | 2.0 | 2.0 |
| Total | | | | | 20 | 20 | 20 |

:::

REVIEW: Stock concentrations for PURExpress Solution A, Solution B, RNase inhibitor, and DFHBI are not available from the source. These fields are left as — and should be confirmed before publication.

## Assembly

1. Retrieved PURExpress Solution A and Solution B from −20 °C storage and thawed both on ice for 5–10 minutes.
2. Kept all components on ice during reaction assembly. Solution B was handled gently because it contains ribosomes and should not be vortexed.
3. Labeled reaction tubes for two positive +PURE reactions and one no-DNA negative control.
4. Added Solution A, Solution B, RNase inhibitor, DNA template where applicable, nuclease-free water, and DFHBI according to the reaction setup table.
5. Mixed each reaction gently by pipetting up and down 10–15 times until homogeneous and clear.
6. Briefly spun tubes in a minicentrifuge to collect liquid and remove bubbles, then held assembled reactions on ice before plating.

## Plating and plate reader setup

1. Transferred reactions to a black 384-well optical plate according to the assigned plate map.
2. Used technical duplicate wells for positive reactions when possible and included the no-DNA control.
3. Measured fluorescence kinetics for approximately 4 hours. Plate reader settings: excitation 485 nm, emission 528 nm, 30 °C, reads every 5–10 minutes.

REVIEW: Exact read interval (5 or 10 minutes) was not specified in the source — confirm from raw data file `team3-graph-data-with-layout.xlsx`.

# Results

Fluorescence was tracked over 4 hours for both the RNA aptamer signal and mScarlet protein production. The plotted data showed increasing fluorescence in the positive reactions, while the no-DNA controls remained close to baseline. This supports successful transcription and translation in the PURExpress reaction and confirms that the observed signal was template-dependent.

:::{figure} figures/kinetics-broccoli-mscarlet.png
:label: fig-kinetics
:align: center
:width: 75%
Broccoli 2 (48.4 ng/µL) and mScarlet fluorescence kinetics in a PURExpress CFPS reaction. Broccoli fluorescence was monitored as a readout of RNA aptamer transcription, while mScarlet fluorescence was monitored as a readout of protein production.
:::

REVIEW: Source figure was embedded in Word document as `media/image1.png`. Confirm that `figures/kinetics-broccoli-mscarlet.png` is the correct extracted file. A notebook (`broccoli-mscarlet-kinetics-graph.ipynb`) and source data (`team3-graph-data-with-layout.xlsx`) are present — consider regenerating the figure from the notebook and embedding via glue rather than using a static PNG.

# Conclusions and next steps

These results demonstrate that a standard PURExpress cell-free protein synthesis reaction can support simultaneous RNA aptamer transcription and protein translation, as detected by real-time Broccoli 2 and mScarlet fluorescence over 4 hours. The no-DNA negative control confirmed that observed signal was template-dependent. Future work will test cytosol performance inside membrane compartments as part of the synthetic-cell assembly workflow.

# References

- CHEM 471 Engineering Synthetic Cells Laboratory Manual, Experiment 1 — Cytosol Assembly. California Polytechnic University, San Luis Obispo.