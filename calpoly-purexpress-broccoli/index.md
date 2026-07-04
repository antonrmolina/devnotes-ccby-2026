---
title: PURExpress Cytosol Assembly with Broccoli 2/mScarlet Reporter
description: |
  A PURExpress cell-free protein synthesis reaction was assembled with a Broccoli 2 RNA aptamer and mScarlet reporter plasmid to test whether transcription and translation could be detected in real time by fluorescence kinetics in a defined reconstituted cytosol. Fluorescence in positive reactions increased over four hours while no-DNA controls remained near baseline, confirming template-dependent expression.
date: 2026-04-03
authors:
  - name: Emily Cook
    affiliation: California Polytechnic University, San Luis Obispo
    email: ecook11@calpoly.edu
  - name: Suna Nguyen
    affiliation: California Polytechnic University, San Luis Obispo
    email: snguy230@calpoly.edu
keywords:
  - cell-free protein synthesis
  - PURExpress
  - Broccoli 2
  - mScarlet
  - RNA aptamer
  - synthetic cell
license: CC-BY-4.0
thumbnail: figures/kinetics-broccoli-mscarlet.png
collections:
  - REVIEW: inferred — CHEM 471 Synthetic Cells coursework
id: dn-2026-ccby-purexpress-cytosol-assembly-broccoli2-mscarlet
---

# Context

This DevNote characterizes a standard PURExpress cell-free protein synthesis reaction using a Broccoli 2 RNA aptamer and mScarlet reporter plasmid. The goal was to test whether transcription and translation could be detected in real time by fluorescence in a defined reconstituted cytosol. The reaction used the CP/CK energy regeneration system built into standard PURExpress Solution A and included a no-DNA negative control to confirm that fluorescence depended on template-driven expression rather than background or instrument noise. This experiment follows the CHEM 471 Experiment 1 cytosol assembly workflow and supports later synthetic-cell work where cytosol performance is tested inside membrane compartments.

# Methods

## Reagents

| Reagent | Product name | Manufacturer | Storage conditions |
|---|---|---|---|
| PURExpress Solution A | PURExpress Solution A with CP/CK energy system | New England Biolabs | -20 °C; thaw and hold on ice |
| PURExpress Solution B | PURExpress ribosome solution | New England Biolabs | -20 °C; thaw and hold on ice; do not vortex |
| RNase inhibitor | RNase inhibitor | — | — |
| DNA template | Broccoli 2 mScarlet, 48.4 ng/µL stock | — | — |
| DFHBI | Fluorogen for Broccoli aptamer | — | — |
| Nuclease-free H2O | Nuclease-free water | — | — |
| 384-well plate | Black optical 384-well plate | — | — |

Catalog numbers and pricing were not recorded in the source materials.

## Reaction composition

Two conditions were prepared: a positive reaction containing DNA template (+PURE, assembled in biological duplicate) and a no-DNA negative control. Because the two +PURE replicates were assembled identically, a single representative table is shown.

::::{tab-set}

:::{tab-item} +PURE reaction (Rep 1 and Rep 2)

| Component | Input concentration | Unit | Final concentration | Unit | Volume (µL) |
|---|---|---|---|---|---|
| Solution A | — | — | — | — | 8.0 |
| Solution B | — | — | — | — | 6.0 |
| RNase inhibitor | — | — | — | — | 0.5 |
| DNA template: Broccoli 2 mScarlet | 48.4 | ng/µL | ~5 | ng/µL | 2.1 |
| Nuclease-free H2O | — | — | — | — | 1.43 |
| DFHBI | — | — | — | — | 2.0 |
| Total | | | | | 20.0 |

:::

:::{tab-item} No-DNA control

| Component | Input concentration | Unit | Final concentration | Unit | Volume (µL) |
|---|---|---|---|---|---|
| Solution A | — | — | — | — | 8.0 |
| Solution B | — | — | — | — | 6.0 |
| RNase inhibitor | — | — | — | — | 0.5 |
| DNA template: Broccoli 2 mScarlet | — | — | — | — | 0 |
| Nuclease-free H2O | — | — | — | — | 3.5 |
| DFHBI | — | — | — | — | 2.0 |
| Total | | | | | 20.0 |

:::

::::

## Assembly

PURExpress Solution A and Solution B were retrieved from -20 °C storage and thawed both on ice for 5-10 minutes. All components were kept on ice during reaction assembly. Solution B was handled gently because it contains ribosomes and should not be vortexed. Reaction tubes were labeled for two positive +PURE reactions and one no-DNA negative control. Solution A, Solution B, RNase inhibitor, DNA template where applicable, nuclease-free water, and DFHBI were added according to the reaction setup table. Each reaction was mixed gently by pipetting up and down 10-15 times until homogeneous and clear. Tubes were briefly spun in a minicentrifuge to collect liquid and remove bubbles, then assembled reactions were held on ice before plating.

## Plate reader setup

Reactions were transferred to a black 384-well optical plate according to the assigned plate map. Technical duplicate wells were used for positive reactions when possible and the no-DNA control was included. Fluorescence kinetics were measured for approximately 4 hours. The lab manual plate reader settings for this experiment were excitation 485 nm, emission 528 nm, 30 °C, and reads every 5-10 minutes.

Raw fluorescence data and the plate layout are provided in `team3-graph-data-with-layout.xlsx`. Kinetics curves were plotted using the Jupyter notebook `broccoli-mscarlet-kinetics-graph.ipynb`, which contains pre-committed PNG output. **REVIEW:** Cell 0 of the notebook raises a runtime error; the pre-committed figure output should be treated as definitive until the runtime issue is resolved.

# Results

:::{figure} figures/kinetics-broccoli-mscarlet.png
:label: fig-kinetics
:width: 75%
Broccoli 2 (48.4 ng/µL) and mScarlet fluorescence kinetics in a PURExpress CFPS reaction. Broccoli fluorescence was monitored as a readout of RNA aptamer transcription, while mScarlet fluorescence was monitored as a readout of protein production. **REVIEW:** "48.4 ng/µL" is the stock concentration; the final concentration in the reaction was approximately 5 ng/µL. Caption should be updated to reflect the final concentration before publication.
:::

Fluorescence was tracked over 4 hours for both the RNA aptamer signal and mScarlet protein production ({ref}`fig-kinetics`). The plotted data showed increasing fluorescence in the positive reactions, while the no-DNA controls remained close to baseline. This supports successful transcription and translation in the PURExpress reaction and confirms that the observed signal was template-dependent.

# Specification

The following parameters are sufficient to reproduce the core experiment:

| Parameter | Value |
|---|---|
| CFPS system | PURExpress (NEB); Solution A with CP/CK energy regeneration |
| Reaction volume | 20 µL |
| DNA template | Broccoli 2 mScarlet plasmid |
| DNA template stock concentration | 48.4 ng/µL |
| DNA template volume | 2.1 µL (+PURE); 0 µL (no-DNA control) |
| DNA template final concentration | ~5 ng/µL |
| Fluorogen | DFHBI, 2.0 µL per reaction |
| Plate format | Black 384-well optical plate |
| Incubation temperature | 30 °C |
| Read duration | ~4 hours |
| Read interval | 5-10 minutes |
| Excitation wavelength | 485 nm |
| Emission wavelength | 528 nm |

Raw data: `team3-graph-data-with-layout.xlsx` (fluorescence readings and plate layout).

Analysis code: `broccoli-mscarlet-kinetics-graph.ipynb` (plots kinetics curves; contains a runtime error in cell 0 — see REVIEW flag in Methods).

# References

- CHEM 471 Engineering Synthetic Cells Laboratory Manual, Experiment 1 — Cytosol Assembly. California Polytechnic University, San Luis Obispo.
