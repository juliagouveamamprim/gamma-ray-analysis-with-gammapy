# Gammapy Tutorials for Gamma-Ray Analysis

Educational notebooks for high-level gamma-ray data analysis with Gammapy.

These tutorials were prepared for the short course "Introduction to Gammapy for Dark Matter Searches", taught at the International Institute of Physics, Universidade Federal do Rio Grande do Norte, in August 2025.

## Contents

The notebooks are available in the notebooks/ directory:

- 01_1d_point_source_analysis.ipynb: spectral analysis of a point-like gamma-ray source.
- 02_3d_gamma_ray_analysis.ipynb: 3D gamma-ray analysis with spatial and spectral modeling.
- 03_dark_matter_simulation.ipynb: introductory dark matter simulation example.

## How to use

Clone this repository and open the notebooks with JupyterLab, Jupyter Notebook, VS Code, or another notebook interface. For example, with JupyterLab:

    git clone https://github.com/juliagouveamamprim/gammapy-tutorial-Natal.git
    cd gammapy-tutorial-Natal
    jupyter lab

The notebooks are designed to be followed in order, but they can also be opened independently depending on the user's background and interests:

1. Start with the 1D point-source analysis notebook.
2. Continue with the 3D gamma-ray analysis notebook.
3. Finish with the dark matter simulation notebook.

Each notebook contains explanatory text and code cells intended for hands-on learning.

## Environment

These tutorials were prepared with Gammapy v1.3.

The recommended installation method is to use the official Gammapy conda environment:

    curl -O https://gammapy.org/download/install/gammapy-1.3-environment.yml
    conda env create -f gammapy-1.3-environment.yml
    conda activate gammapy-1.3

Check the installation with:

    gammapy info

## Gammapy datasets

The notebooks use the public Gammapy datasets.

After activating the environment, download them with:

    gammapy download datasets

Then set the GAMMAPY_DATA environment variable. One option is:

    export GAMMAPY_DATA=$PWD/gammapy-datasets/1.3

You can check whether the data path is available with:

    echo $GAMMAPY_DATA

## Notes

This repository is intended as educational material for hands-on learning. It is not a production analysis pipeline.
