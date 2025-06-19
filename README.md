# mr_ml_boilerplate

A Cookiecutter template for quickly setting up a basic machine learning project with best practices, modular structure, and reproducibility.

## Requirements

- [Cookiecutter](https://cookiecutter.readthedocs.io/en/latest/):  

  Install via pip if you don't have it:
  ```bash
  pip install cookiecutter
  ```

## Usage

### 1. Create a New Project Using This Template

You can use either the GitHub HTTPS URL or your local path:

**From GitHub:**
```bash
cookiecutter https://github.com/Mathanraj-Sharma/mr_ml_boilerplate.git
```

**From a Local Path (if you have cloned the repo):**
```bash
cookiecutter path/to/mr_ml_boilerplate
```

You will be prompted to enter some information about your new project (such as project name, author, etc.).

### 2. Project Structure

Your new project will look like:

```
your_project_name/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── src/
│   ├── __init__.py
│   └── train.py
│   └── test.py
│   └── validation.py
│   └── utils.py
├── tests/
│   ├── __init__.py
│   └── test.py
├── models/
├── requirements.txt
├── Makefile
├── README.md
└── .gitignore
```
## 📦 Tracking Empty Folders with `.gitkeep`

Git does not track empty folders. To ensure critical directories like `models/`, `data/raw/`, and `data/processed/` are preserved in version control (even if initially empty), this template includes `.gitkeep` files inside them.

- `models/.gitkeep`: Placeholder to keep the directory for saved models.
- `data/raw/.gitkeep`: Placeholder to indicate where raw data should be placed.
- `data/processed/.gitkeep`: Placeholder for processed datasets.

You can safely delete these `.gitkeep` files once the directories contain actual files.

## Customization

- Update `requirements.txt` with your dependencies.
- Add custom scripts and notebooks to the respective directories.
- Modify or extend the Makefile for your workflow.

## Contributing

Feel free to fork this template and submit pull requests to improve it!

## License

[Apache License](LICENSE)