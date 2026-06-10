# Setting Up Environment with uv

## Prerequisites
- Python 3.12 or higher installed

## Installation Steps

### 1. Install uv (https://docs.astral.sh/uv/getting-started/installation/#pypi)

**On macOS/Linux:**
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```
**On Windows:**
```bash
winget install --id=astral-sh.uv  -e
```

### 2. Create Virtual Environment
```bash
uv venv -n .venv-cs4603
```

This creates a `.venv-cs4603` directory in your project.

### 3. Activate Virtual Environment

**On macOS/Linux:**
```bash
source .venv-cs4603/bin/activate
```

**On Windows:**
```bash
.venv-cs4603\Scripts\activate
```

### 4. Install Dependencies
```bash
uv pip install -r requirements.txt
```

### 5. Verify Environment
```bash
uv pip list
```

## Quick Reference

| Command | Description |
|---------|------------|
| `uv venv` | Create a new virtual environment |
| `uv pip install` | Install packages |
| `uv pip list` | List installed packages |
| `uv pip freeze` | Generate requirements.txt |