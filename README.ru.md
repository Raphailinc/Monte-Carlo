# Monte Carlo

[![CI](https://github.com/Raphailinc/Monte-Carlo/actions/workflows/ci.yml/badge.svg)](https://github.com/Raphailinc/Monte-Carlo/actions/workflows/ci.yml)

[English](README.md) · [Русский](README.ru.md)

Учебный проект численных методов: оценка двух интегралов, дисперсии и стандартной ошибки методом Монте-Карло.

## Возможности

- Сравнение генератора NumPy и учебного метода середины квадратов.
- Настройка количества выборок, метода и seed через CLI.
- Вывод оценки интеграла, дисперсии и стандартной ошибки.

## Локальный запуск

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m integral_calculations -n 5000 --method numpy --seed 42
```

## Проверки

```bash
python -m pytest
```

## Условия запуска и границы проекта

Метод середины квадратов включён для изучения и может быстро попадать в короткие циклы. Для основного эксперимента используйте NumPy. Результат зависит от размера выборки и seed.
