---
marp: true
theme: default
paginate: true
---

# Créer un bon `pyproject.toml`

## Introduction

- `pyproject.toml` est un fichier de configuration pour les projets Python.
- Standardisé par PEP 518.
- Centralise les configurations des outils de build et des métadonnées du projet.

---
## Structure de base

```toml
[build-system] #Outils pour construire le projet
requires = ["setuptools", "wheel"]
build-backend = "setuptools.build_meta"

[project] #Metadonnées du projet
name = "example_project"
version = "0.1.0"
description = "An example project"
authors = [{ name = "Your Name", email = "your.email@example.com" }]
requires-python = ">=3.8"
dependencies = []
```

---


## Configuration des dépendances

```toml
[project]
dependencies = [
    "numpy >=1.20",
    "pandas >=1.2"
]

[project.optional-dependencies]
test = [
    "pytest >=6.0"
]

```
dependencies: Liste des dépendances
optional-dependencies: outils de test...