# Gammapy tutorials - High Level Analysis 

Material for the high-level analysis using [Gammapy](https://gammapy.org/).

## Installation
We will use the latest release of Gammapy, v1.3.

The recommended setup is described in the [Gammapy documentation](https://docs.gammapy.org/1.3/getting-started/index.html#getting-started). 
The steps are also summarized here (some additional dependencies might be needed) 

The recommended setup is through conda (with i.e. Miniconda, Anaconda or mamba):

```
curl -O https://gammapy.org/download/install/gammapy-1.3-environment.yml
conda env create -f gammapy-1.3-environment.yml
conda activate gammapy-1.3
```

Then, set `GAMMAPY_DATA` either for the environment through:
```
conda activate gammapy-1.3
conda env config vars set GAMMAPY_DATA=$PWD/gammapy-datasets/1.3
conda activate gammapy-1.3
```

or otherwise add it to your bashrc/bash_profile:
```
export GAMMAPY_DATA=$PWD/gammapy-datasets/1.3
```

**Check your installation**

To check that the gammapy environment is working, open a new terminal and type

```
conda activate gammapy-1.3
gammapy info
```
To further check that you have correctly set up the data folder type

## Datasets
Download the following datasets to be used in the hands-on sessions.

- **Gammapy datasets** should be downloaded through:

```
conda activate gammapy-1.3
gammapy download datasets
```