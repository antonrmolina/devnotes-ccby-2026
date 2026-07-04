# Review notes

**Submitted:** 2026-07-04 05:25 UTC
**License:** CC-BY-4.0

## Automated review flags
- 🟡 **general**: inferred — nucleus-core, cal-poly
- 🟡 **Reagents**: storage conditions not provided |
- 🟡 **Reagents**: source and storage not provided |
- 🟡 **Reagents**: supplier and storage not provided |
- 🔴 **Reaction composition**: Stock concentrations for PURExpress Solution A, Solution B, RNase inhibitor, and DFHBI are not available from the source. These fields are left as — and should be confirmed before publication.
- 🟡 **Plating and plate reader setup**: Exact read interval (5 or 10 minutes) was not specified in the source — confirm from raw data file `team3-graph-data-with-layout.xlsx`.
- 🔴 **Results**: Source figure was embedded in Word document as `media/image1.png`. Confirm that `figures/kinetics-broccoli-mscarlet.png` is the correct extracted file. A notebook (`broccoli-mscarlet-kinetics-graph.ipynb`) and source data (`team3-graph-data-with-layout.xlsx`) are present — consider regenerating the figure from the notebook and embedding via glue rather than using a static PNG.

## Reviewer checklist
- [ ] Science looks sound
- [ ] Figures verified
- [ ] Ready to merge
