# Copilot instructions for this repository

This repository currently contains only a Python virtual environment under `venv/` and no application source files, package metadata, or project configuration. There is no `README.md`, `CONTRIBUTING.md`, `pyproject.toml`, `requirements.txt`, `setup.cfg`, `package.json`, `Makefile`, or test suite checked into the repo at the moment. Treat the workspace as an empty Python project until source files are added.

## Build, test, and lint commands

No project-specific build, test, or lint commands are configured in this repository right now.

- No `pyproject.toml`/`tox`/`nox`/`pytest` configuration is present.
- No `requirements.txt` or lockfile is present.
- No `Makefile`, `justfile`, or CI workflow defines a standard command set.

If project files are later added, keep commands aligned with the actual tooling in the repo instead of assuming a framework. For a Python project, the most likely validation commands would be:

- `./venv/Scripts/python.exe -m pytest` for tests
- `./venv/Scripts/python.exe -m compileall .` for syntax validation
- `./venv/Scripts/python.exe -m pip install -r requirements.txt` for dependency setup when a requirements file is introduced

Do not treat files under `venv/` as project source. The virtual environment is tooling, not application code.

## High-level architecture

There is no application architecture to describe yet because no project code is present outside the environment. The current directory structure is effectively: a single virtual environment used to provide Python tooling, with no app modules, service layer, UI, or data model.

Future Copilot sessions should first confirm whether the repository has been populated with application files before assuming frameworks, folder layout, or runtime patterns.

## Key conventions

- Keep project source files outside `venv/`.
- Do not edit or commit generated virtual-environment files unless a task explicitly requires it.
- Because there are no existing project docs or config files, prefer inspecting the repo for actual source layout before writing new code or making assumptions.
- When a real project is added later, update this file to reflect the actual build/test/lint workflow and architecture rather than relying on generic Python conventions.

## Repository-specific notes

- There are no AI-agent instruction files or custom rules in the repo root (`AGENTS.md`, `CLAUDE.md`, `.cursorrules`, `.windsurfrules`, `.clinerules`, etc.).
- There are no project documents to incorporate from README or CONTRIBUTING files.
- The workspace appears to be a blank or newly initialized Python environment rather than a checked-in codebase.
