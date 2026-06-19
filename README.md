# Gamma-Ray Analysis with Gammapy

Educational tutorial notebooks for high-level gamma-ray data analysis with [Gammapy](https://gammapy.org/).

This repository contains hands-on examples covering 1D spectral analysis, 3D spatial/spectral modeling, and a simulated indirect dark matter search with CTAO-like instrument response functions.

The material was originally prepared for the short course **"Introduction to Gammapy for Dark Matter Searches"**, taught at the International Institute of Physics, Universidade Federal do Rio Grande do Norte, in August 2025. It has since been reorganized as a general tutorial repository for gamma-ray analysis with Gammapy.

## Contents

The notebooks are available in the `notebooks/` directory.

| Notebook | Topic |
|---|---|
| `01_1d_point_source_analysis.ipynb` | 1D spectral analysis of a point-like gamma-ray source using public H.E.S.S. DL3 data |
| `02_3d_gamma_ray_analysis.ipynb` | 3D map analysis with spatial and spectral modeling of an extended gamma-ray source |
| `03_dark_matter_simulation.ipynb` | Simulated dark matter search with a J-factor template and a profile-likelihood upper limit |

The notebooks are designed to be followed in order, but they can also be opened independently depending on the user's background and interests.

## How to use

Clone the repository:

```bash
git clone https://github.com/juliagouveamamprim/gamma-ray-analysis-with-gammapy.git
cd gamma-ray-analysis-with-gammapy
```

Open the notebooks with JupyterLab, Jupyter Notebook, VS Code, or another notebook interface:

```bash
jupyter lab
```

Each notebook contains explanatory text and code cells intended for hands-on learning.

## Environment

These tutorials were prepared with **Gammapy v1.3**.

The recommended installation method is to use the official Gammapy conda environment:

```bash
curl -O https://gammapy.org/download/install/gammapy-1.3-environment.yml
conda env create -f gammapy-1.3-environment.yml
conda activate gammapy-1.3
```

Check the installation with:

```bash
gammapy info
```

## Gammapy datasets

The notebooks use public Gammapy datasets, which are not stored in this repository.

After activating the environment, download the datasets with:

```bash
gammapy download datasets
```

Then set the `GAMMAPY_DATA` environment variable. If the datasets were downloaded inside this repository, one option is:

```bash
export GAMMAPY_DATA=$PWD/gammapy-datasets/1.3
```

Check that the data path is available:

```bash
echo $GAMMAPY_DATA
```

The `gammapy-datasets/` directory should remain local and should not be committed to the repository.

## Notes

This repository is intended as educational material for hands-on learning. It is not a production analysis pipeline and should not be interpreted as an official CTAO sensitivity study.

The dark matter notebook is a simplified pedagogical simulation. A realistic analysis would require a more detailed treatment of the region of interest, background systematics, instrumental response, source confusion, diffuse emission, and statistical coverage.
