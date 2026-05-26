# Text Translation & Sentiment Analysis

Translate non-English movie reviews and run sentiment analysis on them using HuggingFace transformers.

## Prerequisites

- Python >= 3.11
- [`uv`](https://docs.astral.sh/uv/) for dependency and environment management

Install `uv` if you don't have it:

```sh
# macOS / Linux
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## Setup

From the project root:

```sh
uv sync
```

This creates a `.venv/` in the project directory and installs every dependency pinned in `uv.lock` (including `torch`, `transformers`, `sentencepiece`, `sacremoses`, `pandas`, and `ipykernel`).

## Running the notebook

Open `project.ipynb` in your editor of choice (VS Code, JupyterLab, etc.) and select the project's `.venv` as the kernel. The `ipykernel` dependency is already included, so no extra registration step is needed.

To launch JupyterLab directly:

```sh
uv run jupyter lab project.ipynb
```

## Adding a dependency

```sh
uv add <package>
```

This updates `pyproject.toml` and `uv.lock` and installs into `.venv/`.
