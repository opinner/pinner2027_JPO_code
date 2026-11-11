# Research code to Pinner et al., (*in prep.*) <!-- omit in toc -->

[![License MIT license](https://img.shields.io/github/license/opinner/pinner2026_JPO_code)](./LICENSE) <!--- Should automatically start to work once the project is public  [![build](https://github.com/opinner/pinner2026_JPO_code/actions/workflows/main.yml/badge.svg)](https://github.com/opinner/pinner2026_JPO_code/actions/) -->

> [!WARNING]
> This is the associated research code to the **upcoming** publication *Surface-driven near-inertial waves determine the seasonal variability of bottom-near turbulence in the Weddell Sea Bottom Water Gravity Current*  by Pinner & Kanzow.
> Because the publication is still under review, this code is also not yet final. Unused code is not yet fully cleaned up, breaking changes can occur at any time, and the documentation is not yet completed.

> [!NOTE]
> The method to calculate time series of dissipation rates is not part of this repo and is currently refactored to the python package *dissipy* and will be soon available.

<!---
Currently this project still contains messy code, most importantly that the methods are banned to `quarantine/_dissip_time_series/`. 
This repo should solely focus on the paper and the figures/results in there, while the method should be encapsulated in the package dissipy.
Therefore, heavy refactoring is needed. There is even a third repo, where I coded the method originally.
-->

### Reproducibility Setup

To reproduce the project, clone this repository on your machine
```bash
git clone https://github.com/opinner/pinner2027_JPO_code
```
The software environment, including all necessary packages, is documented in a more human-readable way in `pyproject.toml` and down to specific version hashes in `requirements.txt`.
The easiest way is to recreate it, is to have [`uv`](https://docs.astral.sh/uv/0) installed, and then run the terminal command `$ uv venv` to build the project environment 

Afterwards, the environment must be activated on Linux/macOS with: `$ source .venv/bin/activate`.

On windows, the activation of the virtual environment needs to be enabled first, via  
```shell
$ (Set-ExecutionPolicy -Scope Process -ExecutionPolicy RemoteSigned) ; (& .venv\Scripts\Activate.ps1)
```
and then
```shell
.\.venv\Scripts\activate
```

> [!NOTE]
> scripts prefixed with `HPC` were executed on AWI's HPC and are included just for documentary purposes/transparency of the calculations. They will most likely not run in a local environment.


## Contact & Issues

For any questions or issues, please contact me via ole.pinner@awi.de or open an [issue](https://github.com/opinner/pinner2026_JPO_code/issues).

---

&copy; [Ole Pinner](https://github.com/opinner), 2026
