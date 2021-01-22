# Repository infrastructure
This repository constains two scripts/notebooks with the nesecairy code to run the species distribution models (SDM): [preperation.ipynb](https://git.fhict.nl/I344070/datics-butterfly-project/-/blob/development/src/preparation.ipynb) and [model_visualise.ipynb](https://git.fhict.nl/I344070/datics-butterfly-project/-/blob/development/src/model_visualise.ipynb).

### Data preperation:
Here you can find the necessairy steps to prepare the data for the model.

### Modeling:
Here the modeling takes place alongside its visualisations. In this notebook can three different kinds of ANN models, their optimalisations and its visualisations be found.

Here you can see how the SDM functions:

![Model Flow](https://i.ibb.co/2MJW0TH/sdm-pipeline.png "Model Flow")  


# Transferability

## Install the necessary Python libraries

Make sure to have Python 3.8 with pip installed, and head over to the `datics-butterfly-project` repository on your machine. In that folder, open a command line interface, and type in:

### With Python
```
pip install virtualenv
virtualenv env_sdm
env_sdm\Scripts\activate
pip install -r requirements.txt
```

### With Conda
```
conda create --name env_sdm pip python=3.8
conda activate env_sdm
pip install -r requirements.txt
```

This installs all the libraries necessary to run the notebooks smoothly. 

## Download the necessary data files
***NOT RECOMMENDED** It is way easier to just download the raw data files and place them at their designated spots e.g. /data/raw/*

You can also download the necessary data files for the notebooks using DVC. First it is important to have read permissions for the Datics Google Drive, and being invited by e-mail, not by invite link. Then, you can open a command line interface in the `datics-butterfly-project` folder again and type in:
```
dvc pull
```
This downloads all the data to work with the notebooks, and also can be opened by e.g. Excel.