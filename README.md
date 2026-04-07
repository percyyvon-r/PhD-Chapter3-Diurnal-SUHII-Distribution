# PhD-Chapter3-Diurnal-SUHII-Distribution

This repository contains the analysis for Research Question 2.b: SUHII Distribution, focused on Melbourne's Surface Urban Heat Island Intensity (SUHII) during warm-season conditions.

## Key Notebook
- `notebooks/PhD_chapter3_ypinb.ipynb`

## Purpose
The notebook implements a direction-enhanced extraction of the Background Rural Area (BRA) and quantifies SUHII for both daytime and nighttime Land Surface Temperature (LST).

The analysis includes:
- defining the BRA using the Urban Growth Boundary (UGB) and Local Climate Zone (LCZ) D,
- applying the DEASE method to identify turning points in directional LST profiles,
- calculating daytime and nighttime SUHII,
- comparing SUHII across LCZs and Local Government Areas (LGAs),
- examining energy flux relationships using sensible and latent heat flux data,
- evaluating diurnal temperature amplitudes.

## Data
Input files are stored in `data/csv/` and include:
- `01_constructed_buffer_metadata_500.csv`
- `02_a_day_lst_500m.csv`
- `02_b_night_lst_500m.csv`
- `03_lst_suhi_zonal_csv.csv`
- `04_a_daytime_BRA_metadata_csv.csv`
- `05_sensible_latent_heat_flux.csv`
- additional derived CSVs and LCZ intersection files

## Outputs
Generated outputs include figures and tables in:
- `outputs/figures/`
- `outputs/tables/`

## Requirements
The project uses Python data analysis and plotting libraries. Relevant dependencies are available in `requirements.txt`.

## How to run
1. Open the repository in VS Code or Jupyter.
2. Activate the project environment.
3. Launch `notebooks/PhD_chapter3_ypinb.ipynb`.
4. Run the notebook cells from top to bottom.

> Note: The notebook uses absolute Windows file paths for data input and output. Update these paths if you run the project on a different machine.

## Notes
- The notebook is the main analysis document for this repository.
- For public browsing, this `README.md` provides the entry point and summary.
