# labjackdriver

# Description

A repo containing a QCoDeS-compatible driver for a labjack.

# Installation

Create a `conda` environment from the environment file in the root folder;
```bash
conda env create -f environment.yml
```
Then activate the environment
```bash
conda activate labjackdriver
```
and install `labjackdriver` either non-editably
```bash
pip install .
```
or in editable mode
```bash
pip install -e .
```

# Usage

## Running the tests

If you have gotten `labjackdriver` from source, you may run the tests locally.

Install `labjackdriver` along with its test dependencies into your virtual environment by executing the following in the root folder

```bash
$ pip install .
$ pip install -r test_requirements.txt
```

Then run `pytest` in the `tests` folder.

## Building the documentation

If you have gotten `labjackdriver` from source, you may build the docs locally.

Install `labjackdriver` along with its documentation dependencies into your virtual environment by executing the following in the root folder

```bash
$ pip install .
$ pip install -r docs_requirements.txt
```

You also need to install `pandoc`. If you are using `conda`, that can be achieved by

```bash
$ conda install pandoc
```
else, see [here](https://pandoc.org/installing.html) for pandoc's installation instructions.

Then run `make html` in the `docs` folder. The next time you build the documentation, remember to run `make clean` before you run `make html`.

# Contributing

We welcome contributions, big and small, as well as questions and suggestions for improving `labjackdriver`. Our community strictly adheres to the [Microsoft open source code of conduct](https://opensource.microsoft.com/codeofconduct).
