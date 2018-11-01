# Using virtualenv to isolate developing environments

## Prerequisites

### Install pip
On Debian/Ubuntu:
```
sudo apt install python-pip
sudo apt install python3-pip
```

### Install virtualenv
On Debian/Ubuntu:
```
python pip install --upgrade pip
python3 pip install --upgrade pip
pip install virtualenv
pip3 install virtualenv
sudo /usr/bin/easy_install virtualenv
```
Reference: [link](https://stackoverflow.com/questions/31133050/virtualenv-command-not-found)


## Using virtualenv

### Initialize virtual environment
```
virtualenv <environment's name/directory's name>
```

### Activate virtualenv
```
source virtualenv <environment's name/directory's name>/bin/activate
```
