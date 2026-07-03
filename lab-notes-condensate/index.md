---
title: Spontaneous RNA Condensate Formation During GUV Encapsulation of Poly-A Sequences
description: During routine encapsulation experiments, dense fluorescent foci appeared reproducibly in vesicles containing poly-A RNA above 0.5 mg/mL, suggesting that crowding-driven phase separation may occur under physiologically relevant cytomimetic conditions.
date: 2026-06-01
authors:
  - name: Sarah Chen
    affiliation: Department of Biochemistry, University of Cambridge
keywords: [PURE system, cell-free, synthetic cell, RNA condensates, phase separation]
license: CC-BY-4.0
thumbnail: figures/key-result.png
collections:
  - cambridge-rna-condensate
---

## Context

These are bench notes from a Wednesday afternoon that I didn't expect to turn into anything. I was running a standard GUV encapsulation of our PURE system mix, this time with a Cy3-labeled poly-A(50) oligo added as a passive volume tracer. The idea was simply to confirm encapsulation efficiency before committing reagents to a full eGFP expression run.

About 40 minutes into imaging, I noticed bright puncta forming inside a subset of vesicles — not aggregates stuck to the membrane, but interior foci that were roundish, mobile by Brownian drift, and clearly distinct from the diffuse Cy3 background. My first instinct was contamination or RNA degradation products. But the puncta appeared in ~30% of vesicles above a certain size threshold, and they weren't present in the control wells without poly-A.

A quick literature check suggested this might be crowding-induced liquid-liquid phase separation of the poly-A RNA, possibly nucleated by the PEG-8000 we include in our encapsulation buffer. RNA condensates driven by crowding agents have been reported in bulk {cite}`Maharana2018,Boija2018`, but I haven't seen it documented specifically in the GUV confinement context.

## Methods

No formal protocol deviation — this was the standard DOPC:DOPG (9:1) GUV preparation by PVA gel-assisted swelling that we run every week. The only difference was the addition of Cy3-labeled poly-A(50) RNA (IDT, HPLC-purified) to the PURE system mix at concentrations of 0.1, 0.5, and 1.0 mg/mL.

Imaging was on the Zeiss LSM 980 confocal (40× water objective, NA 1.2). Single-channel acquisition at 561 nm excitation / 580–620 nm emission. No deconvolution applied. Images taken at 5-minute intervals starting immediately after GUVs were transferred to the observation chamber.

For the condensate intensity measurements, I manually selected 12 vesicles that showed clear puncta (>3 foci per vesicle) and tracked mean puncta intensity vs. diffuse cytoplasmic signal over time using a custom FIJI macro. The plotted ratio (puncta intensity / background) is a rough proxy for condensate enrichment, not a calibrated concentration.

FRAP has not been performed yet to confirm liquid-like behavior.

## Results

The 0.1 mg/mL poly-A wells looked clean — uniform Cy3 fluorescence throughout the vesicle lumen, no puncta at any timepoint. The 0.5 and 1.0 mg/mL wells were where things got interesting.

In the 0.5 mg/mL condition, foci appeared in roughly 28% of GUVs. They nucleated gradually — the diffuse background dimmed as material condensed into 2–5 bright spots per vesicle over 20–30 minutes. In the 1.0 mg/mL condition, puncta were more numerous (often >8 per vesicle) and appeared faster, within the first 10 minutes of imaging.

The enrichment ratio in tracked vesicles reached ~4.5× at plateau. Puncta were dynamic — they moved and occasionally fused into larger droplets, consistent with liquid-liquid phase separation rather than irreversible aggregation.

One odd thing: the condensates preferentially formed near the inner membrane leaflet in the early stages before migrating to the interior. Not sure if this is a real membrane-RNA interaction or an imaging artifact from evanescent field effects near the coverslip.

```{figure} figures/key-result.png
:align: center
:width: 85%
RNA condensate enrichment ratio (puncta intensity / cytoplasmic background) over time for 0.5 and 1.0 mg/mL poly-A(50) in GUV-encapsulated PURE system.
```

## Specification

| Parameter | Value |
|---|---|
| Lipid composition | DOPC:DOPG 9:1 mol/mol |
| Swelling buffer | 300 mOsm sucrose, 10 mM HEPES pH 7.4, 4% PEG-8000 |
| RNA species | Poly-A(50), Cy3-labeled, IDT, HPLC-purified |
| RNA concentrations tested | 0.1, 0.5, 1.0 mg/mL |
| Objective | 40× water, NA 1.2 |
| Excitation | 561 nm |
| Emission | 580–620 nm |
| Imaging interval | 5 min |
| Total imaging duration | 90 min |
| Temperature | ~22–24 °C (ambient, uncontrolled) |
| Condensate foci threshold | >3 foci per vesicle |
| Vesicles tracked for kinetics | 12 |
| Peak enrichment ratio | ~4.5× |
| FRAP performed | No (pending) |

> Temperature was not actively controlled in this experiment. All follow-up experiments should use the stage incubator.
