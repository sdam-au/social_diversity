# Division of Labor and Occupational Specialization and Diversification in the Ancient Roman Cities

This repository contains analyses associated with the article "Division of Labor and Occupational Specialization and Diversification in the Ancient Roman Cities", currently under review (March 2022). It contains scripts, data and figures. The scripts are in Python 3 programming language and have form of Jupyter notebooks. All our analyses aim at being fully reproducible and we invite other scholars to reuse our code and data for their analyses.

---
## Authors
* Vojtech Kase [![](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-6601-1605), SDAM project, kase@kfi.zcu.cz
* Petra Hermankova [![](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-6349-0540), SDAM project, petra.hermankova@cas.au.dk
* Adela Sobotkova [![](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-4541-3963), SDAM project, adela@cas.au.dk

## Abstract
Recent empirical studies on the division of labor in modern cities indicate a complex web of relationships between sectoral specialization of cities and their productivity on one hand and sectoral diversification and resilience on the other. Emerging scholarly consensus suggests that ancient urbanism has more in common with modern urban development than previously thought. We explore whether modern trends in urban division of labor apply to the cities of the Western Roman Empire from the first century BCE to the fourth century CE. We introduce analyses based on occupational data extracted from a large body of Latin epigraphic evidence by computer-assisted text-mining, subsequently mapped onto a dataset of ancient Roman cities. We detect a higher frequency of occupation terms on inscriptions from cities than from rural areas and identify an accumulation of tertiary sector occupations in large cities. The temporal dimension of epigraphic data allows us to study aspects of the division of labor diachronically and to detect trends in the data in a four centuries-long period of Roman imperial history. Our analyses reveal an overall decrease in the frequency of occupational terms between the first half and second half of the third century CE; the maximum frequency of occupational terms shifts over time from large cities to medium and small towns, and finally, rural areas. Our results regarding the specialization and diversity of cities and their respective impact on productivity and resilience remain inconclusive, possibly as a result of the socio-economic bias of Latin inscriptions and insufficient representativeness of the data. Yet, we believe that our formalized approach to the research problem opens up new avenues for research, both in respect to the economic history of the Roman Empire and to the current trends in the science of cities.

---

## License
CC-BY-SA 4.0, see attached [License.md](https://github.com/sdam-au/EDCS_ETL/blob/master/LICENSE.md)

## DOI
Preprint: https://osf.io/preprints/socarxiv/47frj/

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

