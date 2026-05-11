# pyinit

Minimal CLI to initialize modern Python projects for Data Science using `uv`.

## Features

- Initializes Git
- Creates `pyproject.toml`
- Creates `.venv`
- Installs:
  - numpy
  - pandas
  - matplotlib
  - ipykernel
  - ruff
  - pytest
- Generates:
  - `.gitignore`
  - `ruff.toml`
  - `.vscode/settings.json`
- Optional IDE auto-open:
  - Cursor
  - VSCode

---

# Requirements

- Python
- Git
- `uv`

Install `uv`:

```bash
pip install uv
```

---

# Installation

```bash
mkdir -p ~/.local/bin
nano ~/.local/bin/pyinit
chmod +x ~/.local/bin/pyinit
```

Add to PATH:

```bash
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

---

# Usage

Create project:

```bash
pyinit my_project
```

Open in Cursor:

```bash
pyinit my_project --ide cursor
```

Open in VSCode:

```bash
pyinit my_project --ide vscode
```

Initialize current directory:

```bash
pyinit
```

---

# Activate Environment

```bash
source .venv/Scripts/activate
```