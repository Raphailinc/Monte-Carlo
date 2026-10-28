# Monte Carlo

[![CI](https://github.com/Raphailinc/Monte-Carlo/actions/workflows/ci.yml/badge.svg)](https://github.com/Raphailinc/Monte-Carlo/actions/workflows/ci.yml)

[English](README.md) · [Русский](README.ru.md)

A numerical-methods learning project that estimates two demonstration integrals and reports sampling variance and standard error.

## What it does

- Compare a NumPy random generator with an educational middle-square generator.
- Set the sample count, method and seed through the CLI.
- Inspect integral estimates, variance and standard error.

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m integral_calculations -n 5000 --method numpy --seed 42
```

## Checks

```bash
python -m pytest
```

## Scope and implementation notes

The middle-square method is included for study and can have short cycles. Use the NumPy path for the default experiment; results vary with sampling parameters.
