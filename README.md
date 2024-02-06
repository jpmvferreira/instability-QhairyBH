# About

This repository has the simulation parameter files and analysis for the paper entitled "Spontaneous spherical symmetry breaking of black holes with resonant hair".

# Folder structure

- `analyze/`: Jupyter notebooks to analyze simulation output.
- `bin/`: External repository to a set of scripts to manage Einstein Toolkit installations and simulations.
- `env/`: Reproducible virtual environment.
- `notebooks/`: Notebooks to perform auxiliary computations, usually using Wolfram Mathematica (version 14 or higher).
- `par/`: The parfiles provided to the Einstein Toolkit
- `simulations/`: Simulation output data, using [simfactory](https://docs.einsteintoolkit.org/et-docs/Simulation_Factory_Advanced_Tutorial) conventions.

# Reproducibility

To reproduce the contents of this repository there are two things to take into account:
- The Einstein Toolkit installation.
- The Python virtual environment used for the data analysis.

To reproduce the installation of the toolkit, refer to the instructions in [einsteintoolkit.org](https://einsteintoolkit.org/index.html) but use the thornlist provided in `env/thornlist.th` instead. If you face issues compiling the toolkit in your machine, I have a personal directory of options files for the toolkit in [jpmvferreira/cactus-options](https://github.com/jpmvferreira/cactus-options) which might help.

For the Python installation, you can use [conda](https://anaconda.org/channels/anaconda/packages/conda/overview) (or any drop-in replacement like [miniconda](https://www.anaconda.com/docs/getting-started/miniconda/main), [mamba](https://mamba.readthedocs.io/en/latest/) or [micromamba](https://mamba.readthedocs.io/en/latest/user_guide/micromamba.html)) to reproduce the Python virtual environment provided in `env/venv.yaml`. Further packages managed by pip are available in `env/requirements.txt`.

Not all of the simulation data is available in `simulations` due to its large size, but after the previous steps you should be able to reproduce the runs by running the parfile inside each directory.

# Citation

If you used the contents of this repository, please acknowledge it in your work by citing the following reference
```
@misc{Ferreira2026,
  title={Spontaneous spherical symmetry breaking of black holes with resonant hair},
  author={José Ferreira and Carlos A. R. Herdeiro and Eugen Radu and Miguel Zilhão},
  year={2026},
  eprint={2604.22437},
  archivePrefix={arXiv},
  primaryClass={gr-qc},
  url={https://arxiv.org/abs/2604.22437},
}
```

# Contact

For any question regarding the usage of the contents in this repository, feel free to send me an e-mail at [jpmferreira@ua.pt](mailto:jpmferreira@ua.pt).

# License
[MIT](./LICENSE.md)
