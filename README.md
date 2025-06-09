# Alpha_Agent

## Installation

This project uses [uv](https://github.com/astral-sh/uv) to manage Python dependencies. `uv` is a fast, drop-in replacement for pip and virtualenv.

### 1. Install `uv`

You can install `uv` using pipx or pip:

```sh
pipx install uv
# or
pip install uv
```

For more installation options, see the [uv documentation](https://github.com/astral-sh/uv#installation).


### 2. Install dependencies

To install all dependencies defined in `pyproject.toml`, run:

```sh
uv pip install -r pyproject.toml
```

Or, to create a virtual environment and install dependencies:

```sh
uv venv
uv pip install -r pyproject.toml
```

### 3. Activating the virtual environment

On Windows:
```sh
.venv\Scripts\activate
```

On Unix or MacOS:
```sh
source .venv/bin/activate
```

You are now ready to use the project!

## Code Quality: Linting & Formatting with Ruff

This project uses [Ruff](https://docs.astral.sh/ruff/) for all linting, formatting, and import sorting tasks.

### Linting your code

To check your code for errors, style issues, and best practices, run:

```sh
ruff check src
```

### Formatting your code

To automatically format your code according to best practices, run:

```sh
ruff format src
```

### Sorting imports

Ruff also sorts imports for you:

```sh
ruff check src --select I --fix
```

For more options and advanced usage, see the [Ruff documentation](https://docs.astral.sh/ruff/).