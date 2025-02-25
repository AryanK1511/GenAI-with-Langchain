# Conda Cheatsheet

## Conda Basics

```sh
conda info          # Show general conda information
conda --version     # Check Conda version
conda update conda  # Update Conda itself
```

## Managing Environments

```sh
conda create --name my_env python=3.10    # Create a new environment with Python 3.10
conda activate my_env                     # Activate an environment
conda deactivate                          # Deactivate the current environment
conda env list                            # List all environments
conda remove --name my_env                # Delete an environment
```

## Managing Packages

```sh
conda list                                 # List installed packages in the active environment
conda search package_name                  # Search for a package
conda install package_name                 # Install a package in the active environment
conda install -n my_env package_name       # Install a package in a specific environment
conda update package_name                  # Update a package
conda update --all                         # Update all packages in the environment
conda remove package_name                  # Remove a package
```

## Managing Dependencies

```sh
conda clean --all                          # Remove unused packages and cache
conda list --revisions                     # Show environment revision history
conda install package_name=version         # Install a specific package version
conda install package_name=version --freeze-installed  # Avoid updating dependencies
```

## Managing Environment Files

```sh
conda env export > environment.yml         # Export the environment to a YAML file
conda env create -f environment.yml        # Create an environment from a YAML file
conda env update -f environment.yml        # Update an environment from a YAML file
```

## Running Conda from a Different Environment

```sh
conda run -n my_env python script.py       # Run a script using a specific environment
```

## Managing Channels (Repositories)

```sh
conda config --show-sources                # Show configured channels
conda config --add channels conda-forge    # Add a new package source
conda config --set channel_priority strict # Ensure priority order of channels
```

## Conda vs. Pip

```sh
conda install numpy                        # Install using Conda (recommended for scientific packages)
pip install numpy                          # Install using Pip (only inside a virtualenv or Conda env)
conda install pip                          # Install Pip inside a Conda environment
```
