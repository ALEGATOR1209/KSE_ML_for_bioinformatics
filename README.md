# Machine Learning for Bioinformatics

Teaching materials for the KSE course. This repository contains the currently released student materials. Future practicals will be added week by week.

## Repository structure

```text
.
├── pyproject.toml
├── uv.lock
├── .python-version
├── lectures/
│   ├── week1/
│   └── week2/
└── practicals/
    ├── week1/
    └── week2/            
```

Install uv on Windows


```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```


macOS with Homebrew:

```bash
brew install uv
```

macOS without Homebrew:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Linux:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

After installing, close and reopen the terminal, then check that `uv` works:

```bash
uv --version
```

## Create the course environment

From the repository root:

```powershell
uv sync
```

This creates or updates the project environment in `.venv` using the versions recorded in `uv.lock`. The `.venv` directory should not be committed to GitHub.

Start JupyterLab with:
