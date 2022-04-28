# Division of Labor and Occupational Specialization and Diversification in the Ancient Roman Cities

This repository contains analyses associated with the article "Division of Labor and Occupational Specialization and Diversification in the Ancient Roman Cities", currently under review (March 2022). It contains scripts, data and figures. The scripts are in Python 3 programming language and have form of Jupyter notebooks. All our analyses aim at being fully reproducible and we invite other scholars to reuse our code and data for their analyses.

---
## Authors
* Vojtech Kase [![](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-6601-1605), SDAM project, kase@kfi.zcu.cz
* Petra Hermankova [![](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-6349-0540), SDAM project, petra.hermankova@cas.au.dk
* Adela Sobotkova [![](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-4541-3963), SDAM project, adela@cas.au.dk

## Abstract
Recent empirical studies on the division of labor in modern cities indicate a complex web of relationships between sectoral specialization of cities and their productivity on the one hand and its sectoral diversification and resilience on the other. At the same time, an emerging scholarly consensus suggests that modern cities and cities of the past studied by historians and archeologists share a number of  features. Drawing on these debates, we explore to what extent are the observations on the division of labor in modern cities valid for the cities of the Western Roman Empire from the first century BCE to the fourth century CE. We introduce analyses based on occupational data extracted from a large body of Latin epigraphic evidence by computer-assisted text-mining, subsequently mapped onto an existing dataset of ancient Roman cities. The temporal dimension of epigraphic data allows us to study aspects of the division of labor diachronically and to detect trends in the data in a four centuries-long period of Roman imperial history. However, our results regarding the specialization and diversity of cities and their respective impact on productivity and resilience remain inconclusive, possibly as a result of the socio-economic bias of Latin inscriptions and insufficient representativeness of the data. Yet, we believe that our formalized approach to the research problem opens up new avenues for research, both in respect to the economic history of the Roman Empire and to the current trends in the science of cities.

---

## License
CC-BY-SA 4.0, see attached [License.md](https://github.com/sdam-au/EDCS_ETL/blob/master/LICENSE.md)

## DOI
[Here will be DOI or some other identifier once we have it]


---
## How to use this repository

### Data
[EDCS](http://www.manfredclauss.de/) dataset is accessed and transformed by the series of Python and R scripts in [EDCS ETL repository](https://github.com/sdam-au/EDCS_ETL), created by SDAM project. The latest version of the dataset (as JSON file) can be accessed via Sciencedata.dk or at this link: TBA in January [EDCS_public folder](https://sciencedata.dk/shared/1f5f56d09903fe259c0906add8b3a55e). 

[EDH]() dataset is accessed and transformed by the series of Python and R scripts in [EDH ETL repository](https://github.com/sdam-au/EDH_ETL) and in [EDH exploration repository](https://github.com/sdam-au/EDH_exploration), created by SDAM Project. The latest version of the dataset (as JSON file) can be accessed via Sciencedata.dk or at this link: [EDH_public folder](https://sciencedata.dk/shared/b6b6afdb969d378b70929e86e58ad975)

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

