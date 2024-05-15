# Installation Instructions

## Prerequisites

### Paraver/Dimemas

This script relies on `paramedir` and `Dimemas` being installed and available
through the PATH environment variable.

* `paramedir` available at https://tools.bsc.es/paraver
* `Dimemas` available at https://tools.bsc.es/dimemas

If not already done, install both tools and add them to the PATH environment
variable with:

```bash
export PATH=<paraver-install-dir>/bin:$PATH
export PARAVER_HOME=<paraver-install-dir>
export PATH=<dimemas-install-dir>/bin:$PATH
export DIMEMAS_HOME=<dimemas-install-dir>
```

### Python prerequesities

basicanalysis relies on the following python modules:

- `matplotlib`
- `numpy`
- `pandas`
- `scipy`
- `seaborn`

See `pyproject.toml` for more detailed information on specific supported versions.

The simplest way to install is to first to clone the basicanalysis package to your machine

```bash
git clone https://github.com/bsc-performance-tools/basicanalysis.git
```

And then to install run

```bash
cd basicanalysis
pip install .
```

If you want to develop and make changes to the basicanalysis package use this command instead:

```bash
pip install -e .
```

It is recommended to install basicanalysis inside of a virtual environment.

### Other

The gnuplot output requires gnuplot version 5.0 or higher.
