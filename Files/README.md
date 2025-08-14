This project utilizes two distinct versions of the Chemprop library, each essential for different modeling tasks. Due to incompatibilities between the models, it is necessary to maintain separate Python environments.

# Model Compatibility and Environment Setup

## Task 1 & 2: Chung's Model

For predictive tasks involving Chung's Model, a specific version of Chemprop is required. The compatible environment can be set up using the environment.yml file available in the RxnSolvKSE_ML branch of the yunsiechung/chemprop GitHub repository.

To create and activate the correct environment for these tasks, please follow these steps:

## Clone the repository
1. `git clone https://github.com/yunsiechung/chemprop.git`
2. `cd chemprop`
3. `git checkout RxnSolvKSE_ML`

## Create the conda environment

1. `conda env create -f environment.yml`
2. `conda activate chemprop`

## Task 3: Spiekermann Model

The Spiekermann Model for solvated barrier prediction requires a different version of the Chemprop library. The environment.yml for this task is provided within this repository.

To set up the environment for predicting with the Spiekermann Model, use the following commands:

# Assuming you are in the root of this project directory
# Create the conda environment from the local environment.yml
1. `conda env create -f environment.yml`
2. `conda activate chemprop_spiekermann`

Important Considerations:

It is crucial to switch to the appropriate environment before running predictions for the respective models to avoid errors and ensure accurate results.
The primary difference in the environments lies in the core Chemprop library version and its dependencies. The Chung model is compatible with an older version of Chemprop, while the Spiekermann model requires a more recent or modified version.

Please refer to the official Chemprop documentation for more information on the library and its versions.
