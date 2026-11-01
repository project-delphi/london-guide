# AGENTS.md

## Scope

This project is a London visitor guide for the London tourism office. The guide is written
once, in Markdown/Quarto, and reused for every audience (web page, documents, slides and
other formats). It is not a general travel blog, and it does not cover places outside London.

## Rules

1. **Every number comes from a cited file in `data/`.** Never type a statistic by hand:
   read it from a data file whose rows say where the figure came from.
2. **Photos are openly licensed, credited and show no people.** Use only images with an
   open licence, give the credit (author, licence, source) next to each image, and do not
   use photos in which people can be recognised.
3. **Never invent facts.** If a fact, figure, link or credit cannot be verified from a
   source, leave it out and say so instead of guessing.

## Commands

This folder has its own Python environment, managed with `uv` (`pyproject.toml`, `uv.lock`,
`.venv/`). Always run Quarto and Python through `uv run`, for example
`uv run quarto render london.md`, `uv run quarto preview` or `uv run python script.py`.
Add packages with `uv add <package>`, never with `pip install`.
