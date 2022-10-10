# Zdiab_tools
zdiab-tools is a Python library for preprocessing and automating functions for Rasa NLU
## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install zdiab-tools.

```bash
pip install zdiab-tools
```

## Usage

```python
from zdiab_tools import Automate

### returns 'slot'
Automate.add_slot(name_form, list_slots)

### returns 'conf_file'
Automate.conf_file(path, language='fr', policies=False):

### returns 'pickle file'
Automate.def pickle_action(path):
```
## Function
```python

#######################################
## Fonction pour ajouter avec rasa YAML 
#######################################

def add_rasa_file(yaml_string, path):
def add_intent(name, list_action):
def add_forms(name, list_slots):
def add_slot(name_form, list_slots):
def add_responses(list_name, list_action):
def add_file(path, str):

#####################
## Fonction ALTER !!!
#####################

def alter_intent(name, list_action):
def alter_slot(name_form, list_slots):
def alter_forms(name, list_slots):
def alter_responses(list_name, list_action):
def alter_file(path, li, required=False):

############################################
## Fonction pour AJOUTER NLU DATA ##########
############################################

def add_nluData(name_intent, list_exemple, head=False):

############################################
## Fonction pour Alter Config FILE #########
############################################

def conf_file(path, language='fr', policies=False):

############################################
## Fonction Create and Save Action FILE ####
############################################

def pickle_action(path):
def Action_file(path, filename="test.pkl"):

```
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
