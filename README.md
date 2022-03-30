# Associations in Latin inscriptions

This repository contains scripts analysing associations in the Western Roman Empire. More details will follow.

---
## Authors (ordered alphabetically)
* Petra Hermankova [![](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-6349-0540), SDAM project, petra.hermankova@cas.au.dk
* Vojtech Kase [![](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-6601-1605), SDAM project, kase@kfi.zcu.cz
* Adela Sobotkova [![](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-4541-3963), SDAM project, adela@cas.au.dk

## Abstract
TBA
---

## License
CC-BY-SA 4.0, see attached [License.md](https://github.com/sdam-au/EDCS_ETL/blob/master/LICENSE.md)

## DOI
TBA

---
## How to use this repository

### Data
Latin Inscriptions of the Roman Empire (LIRE) dataset created by series of scripts in [LIRE_ETL](https://github.com/sdam-au/LIRE_ETL) repository and published on Zenodo https://zenodo.org/record/5776109

**The LIRE dataset** is an aggregate of EDH and EDCS epigraphic datasets, focusing on inscriptions which are (a) geolocated, (b) within the borders of the Roman Empire in its highest extent, (c) dated (d) in the dating interval intersecting the period from 50 BC to 350 AD. In version 1.2, the dataset consists of 136,190 records and 112 attributes. There are 48,801 inscriptions shared by the EDH and EDCS, inheriting attributes from both parent collections. Further, there are 3,907 inscriptions recorded exclusively in EDH and 83,482 inscriptions originating solely from EDCS. In cases in which an inscription is available only in one dataset, it contains attributes only from that one dataset. 

We publish the dataset as one geojson file. The scripts used to generate the dataset and their metadata are available via GitHub:  https://github.com/sdam-au/LIRE_ETL.

The LIRE dataset has been created aggregating the following datasets: 
- [EDH](https://edh-www.adw.uni-heidelberg.de/) dataset is accessed and transformed by the series of Python and R scripts in [EDH ETL repository](https://github.com/sdam-au/EDH_ETL) created by the SDAM Project. The latest version of the dataset (as JSON file) can be accessed via Sciencedata.dk or at this link: [EDH_public folder](https://sciencedata.dk/shared/b6b6afdb969d378b70929e86e58ad975)

- [EDCS](http://www.manfredclauss.de/) dataset is accessed and transformed by the series of Python and R scripts in [EDCS ETL repository](https://github.com/sdam-au/EDCS_ETL), created by the SDAM project. The latest version of the dataset (as JSON file) can be accessed via Sciencedata.dk or at this link: [EDCS_public folder](https://sciencedata.dk/shared/1f5f56d09903fe259c0906add8b3a55e). 



### Software
* Python 3
* Jupyter notebooks app/JupyterLab/JupyterHub
* Python 3 additional libraries listed `requirements.txt`


### Getting Started

* download or clone the repository
* create virtual environment following the instructions below
* in the jupyter notebooks available in `/scripts` subdirectory, always check that you are connected to the `socdiv_venv` kernel
* (alternatively, if you do not wish to use the virtual environment, make sure that you have installed all required python packages within the `requirements.txt` file: `pip install -r requiremnts.txt`)

To create the virtual environment, move into the repository directory in terminal and run the following commands: 
```bash
pip install virtualenv
virtualenv socdiv_venv 
socdiv_venv/bin/python -m pip install -r requirements.txt # install anything in requirements.txt
socdiv_venv/bin/python -m ipykernel install --user --name=socdiv_venv

```
If you have issues, check that you are within the right directory and that your `pip` is coupled with Python 3 (and not Python 2): `pip --version`

