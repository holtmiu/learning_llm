# Learning LLM

This repository is dedicated to learning Large Language Models (LLMs) through practical projects and Kaggle competitions.

## Project Setup

This project uses [uv](https://github.com/astral-sh/uv) for Python package management.

### Prerequisites

- [uv](https://docs.astral.sh/uv/getting-started/installation/) installed on your system.

### Installation

Clone the repository and install dependencies:

```bash
# Sync dependencies and create a virtual environment
uv sync
```

### Common `uv` Commands

- **Add a new package:** `uv add <package_name>`
- **Run a script:** `uv run <script_path>`
- **Run Jupyter Lab:** `uv run jupyter lab`
- **Update dependencies:** `uv lock --upgrade`

## Kaggle Integration

The project includes a dedicated directory for Kaggle competitions: `kaggle/llm-classification-finetuning`.

### Setup Kaggle Credentials

1.  Go to your [Kaggle Account](https://www.kaggle.com/settings) and click **"Create New API Token"**.
2.  Save the `kaggle.json` file to `~/.kaggle/kaggle.json`.
3.  Ensure the file permissions are secure:
    ```bash
    chmod 600 ~/.kaggle/kaggle.json
    ```

### Downloading Datasets

You can use the `kaggle` CLI (installed via `uv`) to download datasets:

```bash
# Example: Download the competition dataset
uv run kaggle competitions download -c llm-classification-finetuning
```

## Project Structure

- `kaggle/`: Contains Kaggle competition-specific code and datasets.
    - `llm-classification-finetuning/`: 
        - `datasets/`: Scripts and storage for datasets.
        - `src/`: Source code for models and analysis.
- `main.py`: Entry point for general LLM experiments.
- `pyproject.toml`: Project configuration and dependencies managed by `uv`.

## License

[MIT](LICENSE) (or specify your license)
