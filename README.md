# Transferability

## Install the necessary Python libraries
Make sure to have Python 3.8 with pip installed, and head over to the `datics-butterfly-project` repository on your machine. In that folder, open a command line interface, and type in:
```
pip install virtualenv
virtualenv env
env\Scripts\activate
pip install -r requirements.txt
```
This installs all the libraries necessary to run the notebooks smoothly. 

## Download the necessary data files
**NOT RECOMMENDED** It is way easier to just download the raw data files and place them at their designated spots (data/raw)

You can also download the necessary data files for the notebooks using DVC. First it is important to have read permissions for the Datics Google Drive, and being invited by e-mail, not by invite link. Then, you can open a command line interface in the `datics-butterfly-project` folder again and type in:
```
dvc pull
```
This downloads all the data to work with the notebooks, and also can be opened by e.g. Excel.