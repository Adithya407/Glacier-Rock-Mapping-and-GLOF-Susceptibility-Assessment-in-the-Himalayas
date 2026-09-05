# Glacier Lake Mapping and GLOF Susceptibility Assessment Using SAR Data

[![Code License: GPL v3](https://img.shields.io/badge/Code%20License-GPLv3-blue.svg)](LICENSE)
[![Data/Docs License: CC BY 4.0](https://img.shields.io/badge/Data%2FDocs%20License-CC%20BY%204.0-lightgrey.svg)](LICENSE-DATA.md)

Research project on mapping glacial lakes and assessing Glacial Lake Outburst Flood (GLOF) susceptibility for a Himalayan study region, using Synthetic Aperture Radar (SAR) and complementary remote sensing data.

## Background

This project was initiated following the 26 August 2026 Nepal–Tibet flash flood, in which a rock-and-ice avalanche off Langtang Lirung dammed the Lhende Khola River with its own debris before the temporary dam failed, triggering a catastrophic downstream flood. The event was not a classic single-mapped-lake GLOF, and it demonstrated that a susceptibility framework built only around existing glacial lake inventories can miss the hazard entirely. Accordingly, this project's scope extends beyond conventional lake-outburst susceptibility to include:

- Rock-ice avalanche / unstable slope source areas that could dam a valley without any pre-existing lake
- Cascading hazard connectivity from source to downstream settlements
- Prediction of where new glacial lakes may form as glaciers continue to retreat

## Research Objectives

1. **Glacial lake inventory** — SAR-based (and optical cross-validated) mapping of existing lakes in the study region, including lakes seasonally masked by snow cover.
2. **Existing-lake GLOF susceptibility** — Multi-criteria susceptibility scoring of mapped lakes (dam type, freeboard, area growth rate, parent glacier condition).
3. **Source-area hazard susceptibility** — Identification of steep rockwall / hanging-glacier / permafrost-degraded slopes prone to failure, independent of any existing lake.
4. **Future lake formation** — Modeling of glacier-bed overdeepenings likely to become new lakes under continued glacier retreat.
5. **Integrated susceptibility map** — Combination of the above layers with downstream drainage connectivity and exposure.
6. **Case-study validation** — Retrospective test of the framework against the August 2026 Langtang Lirung event.

## Data Sources

| Source | Use |
|---|---|
| Bhoonidhi (ISRO) — NISAR L/S-band, RISAT-1/2, Cartosat DEM/stereo | SAR imagery, DEM |
| Sentinel-1 (Copernicus / ASF Vertex) | C-band SAR, lake extraction, offset tracking |
| Sentinel-2 / Landsat | Optical cross-validation |
| ICIMOD Glacial Lake Inventory | Baseline lake inventory, validation |
| RGI (Randolph Glacier Inventory) | Glacier outlines |
| Copernicus GLO-30 / ASTER GDEM / SRTM | DEM, slope, bed-topography inputs |

## Repository Structure
```
.
├── code/                # All source code (scripts, notebooks, pipelines)
│   ├── preprocessing/    # SAR/optical preprocessing
│   ├── lake_extraction/  # Waterbody extraction and classification
│   ├── susceptibility/   # Susceptibility scoring and modeling
│   └── utils/
├── data/                # Derived and processed datasets
├── docs/                # Reports, methodology notes, literature review
├── figures/             # Maps, charts, and other visual outputs
├── LICENSE              # GNU GPLv3 — applies to everything under code/
├── LICENSE-DATA         # CC BY 4.0 — applies to data/, docs/, figures/
└── README.md
```

## Getting Started

> Requirements and setup instructions to be added as the processing pipeline is developed. Anticipated stack: Python (GDAL, rasterio, numpy, scikit-learn), SNAP/ESA toolbox for SAR preprocessing, QGIS for visualization.

```bash
git clone <repository-url>
cd <repository-name>
# setup instructions TBD
```

## License

This repository uses a **dual-license structure**:

- **Code** (everything under `src/`, scripts, notebooks, and other software) is licensed under the **GNU General Public License v3.0 (GPL-3.0)**. See [LICENSE](LICENSE).
- **Scientific data, figures, and documentation** (everything under `data/`, `docs/`, `results/`, this README, and other written material) is licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**. See [LICENSE-DATA.md](LICENSE-DATA.md).

When reusing material from this repository, please apply the license appropriate to the type of material (code vs. data/documentation) and provide attribution as required by CC BY 4.0 where applicable.

## Citation

> Citation details (authors, institution, DOI) to be added once available.

## Acknowledgments

> Project supervisor / institution / department to be added.