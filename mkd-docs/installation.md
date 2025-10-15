# Installation

`pyDOE3` can be installed from `pypi`, `conda-forge`, and `git`.

## [PyPI](https://pypi.org/project/pyDOE3)

For using the PyPI package in your project, you can update your configuration file by adding following snippet.

=== "pyproject.toml"

    ```toml
    [project.dependencies]
    pyDOE3 = "*" # (1)!
    ```

    1. Specifying a version is recommended

=== "requirements.txt"

    ```
    pyDOE3>=0.3.0
    ```

### pip

=== "Installation for user"

    ```bash
    pip install --upgrade --user pyDOE3 # (1)!
    ```

    1. If you have both Python 2 and Python 3 installed, you may need to use `pip3` instead of `pip` to ensure you're installing the package for Python 3. This is much common on GNU/Linux systems.

=== "Installation in virtual environment"

    ```bash
    python -m venv .venv
    source .venv/bin/activate
    pip install --require-virtualenv --upgrade pyDOE3 # (1)!
    ```

    1. If you have both Python 2 and Python 3 installed, you may need to use `pip3` instead of `pip` to ensure you're installing the package for Python 3. This is much common on GNU/Linux systems.

    !!! note
        Command to activate the virtual env depends on your platform and shell. [More info](https://docs.python.org/3/library/venv.html#how-venvs-work)


### pipenv

    ```bash
    pipenv install pyDOE3
    ```

### uv

=== "Adding to uv project"

    ```bash
    uv add pyDOE3
    uv sync
    ```

=== "Installing to uv environment"

    ```bash
    uv venv
    uv pip install pyDOE3
    ```

### poetry

```bash
poetry add pyDOE3
```

### pdm

```bash
pdm add pyDOE3
```

### hatch

```bash
hatch add pyDOE3
```

## [conda-forge](https://anaconda.org/conda-forge/pydoe3)

You can update your environment spec file by adding following snippets.

```yaml title="environment.yml"
channels:
  - conda-forge
dependencies:
  - pyDOE3 # (1)!
```

1. Specifying a version is recommended

Installation can be done using the updated environment spec file.

=== "conda"
    ```bash
    conda env update --file environment.yml
    ```
=== "micromamba"
    ```bash
    micromamba env update --file environment.yml
    ```

!!! note
    replace `environment.yml` with your actual environment spec file name if it's different.

Or directly in your conda environment.

=== "conda"
    ```bash
    conda install -c conda-forge pyDOE3
    ```
=== "micromamba"
    ```bash
    micromamba install -c conda-forge pyDOE3
    ```

## [git](https://github.com/relf/pyDOE3)

Sometimmes release can fall behind the latest changes in the repository. `pip` can directly install from the git repository.

```bash
pip install --upgrade "git+github.com/relf/pyDOE3.git#egg=pyDOE3"
```

## Dependencies

* Python Installation [see supported python versions](https://devguide.python.org/versions/#supported-versions)
* [numpy](https://pypi.org/project/numpy)
* [scipy](https://pypi.org/project/scipy)
