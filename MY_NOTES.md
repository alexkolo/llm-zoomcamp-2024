# Setup

## Local Setup (Win10)

1. Prerequisites

    - WSL install
    - Docker install
        - https://community.chocolatey.org/packages/docker-desktop#individual
        - test: `docker version`

2. Environment

    ```bash
    pyenv global 3.11.9
    python -m venv venv  # removed via: sudo rm -rf venv
    .\venv\Scripts\Activate # alias venv
    pip install -U pip wheel setuptools
    pip install -r requirements.txt
    ```

3. pre-commit

    ```bash
    pip install pre-commit
    pre-commit install
    pre-commit autoupdate
    # pre-commit run # test
    ```

## Sync with upstream fork

- via command line:

    ```bash
    git fetch upstream
    git merge upstream/main
    ```

- via VSCode:
    - handle conflicts
    - commit & push via _Source Control_ GUI

see: https://stackoverflow.com/a/19506355

## GitHub Codespace Setup

- docker is already installed

1. Environment

    ```bash
    pip install -U pip wheel setuptools
    pip install -r requirements.txt
    ```

2. pre-commit

    ```bash
    pip install pre-commit
    pre-commit install
    pre-commit autoupdate
    # pre-commit run # test
    ```

# Homework

## Module 1: Introduction to LLMs and RAG

- [Homework](cohorts\2024\01-intro\homework.md)
    - [Answer](cohorts/2024/01-intro/module01.ipynb)
