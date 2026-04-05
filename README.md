# 📚 CS249r - Machine Learning Systems

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

The official codebase and command-line interface (CLI) tools for building, curating, and deploying the **Machine Learning Systems** textbook. This repository contains the heavily modularized infrastructure required to compile Quarto-based scientific literature into HTML, EPUB, and PDF formats globally.

## 🚀 System Architecture
- **Modular Build CLI**: Contains a custom Python CLI (`main.py`, `build.py`, `doctor.py`) for maintaining textbook health and generating specific chapters.
- **Pandoc / LUA Filters**: Highly specialized `.lua` scripts (`inject_glossary.lua`, `inject_quizzes.lua`) for dynamic document rendering.
- **Containerized Workflows**: Full Docker support (`linux` and `windows` architectures) for reliable cross-platform book deployments and Binder configuration.

## 🛠️ Build The Book
```bash
pip install -r requirements.txt
python cli/main.py build --format html
```
