# Notebook README: PhD_chapter3_ypinb.ipynb

## Overview
This notebook implements the analysis for Research Question 2.b: SUHII Distribution, focusing on the Surface Urban Heat Island Intensity (SUHII) for Melbourne during warm-season conditions.

The notebook:
- defines the Background Rural Area (BRA) using a direction-enhanced adaptive synchronous extraction (DEASE) method,
- calculates SUHII based on daytime and nighttime Land Surface Temperature (LST),
- performs turning point analysis on directional LST gradients,
- explores SUHII spatial distribution across Local Climate Zones (LCZ) and Local Government Areas (LGAs).

## Key Objectives
- Locate the Background Rural Area using mean daytime and nighttime LST from December 2022 and January 2023.
- Compare daytime and nighttime SUHII patterns.
- Examine SUHII distribution by LCZ and LGA.
- Evaluate how the diurnal cycle of LST influences SUHII spatial patterns.

## Data Sources
The notebook reads input data from the repository's `data/csv/` folder, including:
- `01_constructed_buffer_metadata_500.csv`
- `02_a_day_lst_500m.csv`
- `02_b_night_lst_500m.csv`
- Additional intermediate and output CSV files under `data/csv/` as needed.

The analysis is based on STARFM-fused LST imagery representing:
- daytime LST at 30 m resolution,
- nighttime LST at 70 m resolution.

Selected study dates:
- 3 December 2022
- 27 December 2022
- 7 January 2023
- 27 January 2023

## Outputs
The notebook produces outputs in the repository's `outputs/` folder, including:
- figures in `outputs/figures/`
- tables in `outputs/tables/`

It also references a study area method figure at:
- `outputs/figures/study_area_method_jpg.jpg`

## Dependencies
This notebook uses the following Python packages:
- `pandas`
- `numpy`
- `matplotlib`
- `scipy`
- `pygam`

Additional dependencies may be available in the repository `requirements.txt` file.

## How to Run
1. Activate the Python environment used for this project.
2. Open `notebooks/PhD_chapter3_ypinb.ipynb` in Jupyter or VS Code.
3. Run the notebook cells sequentially from the top.

> Tip: The notebook loads data from absolute Windows paths. If you run it on another machine, update the file paths in the first data-loading cells to match your local repository location.

## Notes
- The BRA is defined based on LCZ D (Low Plants) and Melbourne's Urban Growth Boundary (UGB).
- The DEASE method adapts rural reference extraction to each direction using turning points along LST gradient profiles.
- A sensitivity analysis is included to support the smoothing parameter choice used in turning point detection.
