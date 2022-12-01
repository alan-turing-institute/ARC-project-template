# ARC-project-template

**TODO** A description of the project

## Using this template

***⚠️ Delete this section after you're done***

### What this does

### Pre-requisites

- poetry
  - See https://python-poetry.org/docs/#installation for installation instructions

### Setup

1. Create a new repo from this template, with name in the format `ARC-<project-name>`, and clone it locally

2. Edit the lines with `TODO` comments in `pyproject.toml` and `.github/workflows/actions.yml`, including changing the name of the `src/todo_packagename.

3. Update and install Poetry dependencies

   ```bash
   poetry update
   poetry install
   ```

4. Update and install pre-commit hooks:

   ```bash
   poetry run pre-commit autoupdate
   poetry run pre-commit install --install-hooks
   ```

5. Update the README with a description of the project and fill the other sections marked as TODO

## Installation

1. Clone this repository

2. Install with `pip`:

   ```bash
   pip install .
   ```

## Usage

**TODO**

## Development

### Developer Setup

1. Install dependencies with Poetry

   ```bash
   poetry install
   ```

2. Install pre-commit hooks:

   ```bash
   poetry run pre-commit install --install-hooks
   ```

### Common Commands

- To run commands in the poetry virtual environment (in a terminal), either:
  - Prefix the command you want to run with `poetry run`
    - e.g. `poetry run python myscript.py`
  - Enter the virtual environment with `poetry shell` and then run commands as normal
    - then exit the virtual environment with `exit`

- To run tests:

   ```bash
   poetry run pytest
   ```

- To run linters:
  - If you have setup pre-commit `flake8`, `black`, and `isort` will run automatically before making commits
  - Or you can run them manually:

    ```bash
    poetry run black .
    poetry run isort .
    poetry run flake8
    ```
