# Technical Writing Portfolio

Technical writing portfolio by Daniil Krivoshein. It includes formal software documentation, an educational technical report, API documentation, an installation guide, and a knowledge base article.

## Portfolio site

[Open the published portfolio](https://owlildrownit-dev.github.io/Portfolio/)

## Run locally

```bash
python -m venv .venv
python -m pip install -r requirements.txt
python -m mkdocs serve
```

Open `http://127.0.0.1:8000`.

## Build

```bash
python -m mkdocs build --strict
```

Pushes to `main` trigger the GitHub Pages deployment workflow.
