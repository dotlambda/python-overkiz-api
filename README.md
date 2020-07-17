# Somfy TaHoma

<p align=center>
    <a href="https://github.com/iMicknl/python-tahoma-api/actions"><img src="https://github.com/iMicknl/python-tahoma-api/workflows/CI/badge.svg"/></a>
    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
</p>

An updated and async version of the original [tahoma-api](https://github.com/philklei/tahoma-api) by [@philklei](https://github.com/philklei). The aim of this wrapper is to offer an easy to consume Python wrapper for the internal API's used by tahomalink.com.

Somfy TaHoma has an official API, which can be consumed via the [Somfy-open-api](https://github.com/tetienne/somfy-open-api). Unfortunately only a few device classes are supported via the official API, thus the need for this wrapper.

This package is written for the Home Assistant [ha-tahoma](https://github.com/iMicknl/ha-tahoma) integration, but could be used by any Python project interacting with Somfy TaHoma devices.

## Installation

```bash
pip install git+https://github.com/iMicknl/python-tahoma-api.git@master#tahoma_api
```

## Development

### Installation

- For Linux, install [pyenv](https://github.com/pyenv/pyenv) using [pyenv-installer](https://github.com/pyenv/pyenv-installer)
- For MacOS, run `brew install pyenv`
- Don't forget to update your `.bashrc` file (or similar):
  ```
  export PATH="~/.pyenv/bin:$PATH"
  eval "$(pyenv init -)"
  ```
- Install the required [dependencies](https://github.com/pyenv/pyenv/wiki#suggested-build-environment)
- Install [poetry](https://python-poetry.org): `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python`

- Clone this repository
- `cd python-tahoma-api`
- Install the required Python version: `pyenv install 3.8.3`
- Init the project: `poetry install`
- Run `poetry run pre-commit install`

## PyCharm

As IDE you can use [PyCharm](https://www.jetbrains.com/pycharm/).

Using snap, run `snap install pycharm --classic` to install it.

For MacOS, run `brew cask install pycharm-ce`

Once launched, don't create a new project, but open an existing one and select the **python-tahoma-api** folder.

Go to _File | Settings | Project: nre-tag | Project Interpreter_. Your interpreter must look like `<whatever>/python-tahoma-api/.venv/bin/python`
