# ARC-project-template

**TODO** A description of the project

## Using this template

### What this does

This repo has a blank directory structure for an ARC Python project, including setting up:

- `poetry` - for dependencies (including development dependencies) and creating a Python package from your source code
- `pre-commit` - to automatically run linters (`flake8`, `black`, and `isort`) for style checks and auto-formatting
- A GitHub actions workflow to automatically run linters and tests on pushes or pull requests to the `main` and `develop` branches (by default)

### Pre-requisites

- `poetry`
  - See https://python-poetry.org/docs/#installation for installation instructions

### Setup

1. Create a new repo from this template (green button "Use this template" top right -> create new repository), with a name in the format `ARC-<project-name>`, and clone it locally

2. Edit the lines with `TODO` comments in `pyproject.toml` and `.github/workflows/actions.yml`, including changing the name of the `src/todo_packagename` directory.

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

6. Delete the "Using this template" section of this readme, and optionally the file `.github/workflows/update_template.yml`


## Links

- e.g. to report and statement of work (if these can be shared)

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

### Common Commands/Tasks

- To add dependencies to the poetry environment:

   ```bash
   poetry add <PACKAGE_NAME>
   ```

  See [the poetry documentation](https://python-poetry.org/docs/basic-usage/#specifying-dependencies) for more details on specifying dependencies.


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

- Your source code files should go in the `src/todo_packagename` directory (with `todo_packagename` replaced with the name of your package). These will be available as a python package, i.e. you can do `from todo_mypackagename.myfile import myfunction` etc.

- Add tests (in files with names like `test_*.py` and with functions with names starting `test_*`) the `tests/` directory.
