## DOC LINK
https://blog.jayway.com/2019/12/28/pyenv-poetry-saviours-in-the-python-chaos/

---

## PYENV

### Doc link
https://github.com/pyenv/pyenv
https://github.com/pyenv/pyenv-virtualenv

### Install
- list available python version to install `pyenv install --list` 

- install some python version `pyenv install  3.8.13` 

- see installed python version `pyenv versions` 


- python is install in your `$(pyenv root)/versions` directory

### Chose python version

- global way: `pyenv global 3.8.13` set `3.8.13` into `~/.pyenv/version` or do it manualy
- local way: `python local 3.8.13` set `3.8.13` into `./.python-version` or do it manualy

- to see with version is in use: `pyenv version`

- create a virtualenv with pyenv (install pyenv-virtualenv): 
    `pyenv virtualenv 3.8.13 demo-python-project-setup`

- to use python in the system: `pyenv global/local system`

---

## POETRY

### Init
- create a new project: `poetry new DemoPythonProjectSetup`
- init poetry: `poetry init`

### Add dependency
- add dependency: `poetry add pandas`
- for dev env dependency: `poetry add --dev pytest`

### Existing project
- to intall all depencency `poetry install`

### Usage
- create a virtualenv and activate it: `poetry shell`, `exit` to deactivate the env one you are in
- single run on virtualenv: `poetry run pip list`

### Packaging
- bump up version: `poetry version [path, minor, major...]`
- create a wheel package: `poetry build --format wheel`
- upload to a artifactory: `poetry publish --repository XXX --username YYY --password ZZZ [--dry-run]`

### Doc link
https://python-poetry.org/



