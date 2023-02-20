# mtf-data-science-lighthouse

The main objective is to identify which machines will potentially fail and predict their failure type based on data extracted through sensors during the manufacturing process.

![correlation](https://user-images.githubusercontent.com/106438902/220067151-ec586ad7-0569-4d01-99ce-1e106681dfce.png)

This notebook was built for the selection process to participate in Indicium's Lighthouse Program.
## Setup

The code was developed in Windows and the environment created using the `mambaforge` tool (a tool similar to `conda`, but faster and using the `conda-forge` repository). The exact environment may be recreated from the `conda-lock.yml` file. Note that due to a package conflict for `tensorflow`, it is currently using Python 3.7.

A set of `requirements.in` and `requirements.txt` files (created with `pip-tools`) is provided to be used with `pip`, but this wasn't tested.

### Step-by-step to use it with `mambaforge`

* Download the installer from https://github.com/conda-forge/miniforge#mambaforge (for example, the [Mambaforge-Windows-x86_64](https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-Windows-x86_64.exe) version), install it, and start the "Miniforge Prompt".
* Enter the directory where this repository is cloned and execute:

```
$ conda create -n lighthouse --file conda-win-64.lock
```

* Note that lock files for other platforms have been provided.
* Activate the environment and start jupyter with:

```
$ conda activate lighthouse
$ jupyter lab
