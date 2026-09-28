# Analytics Wiki

Личный справочник по аналитике данных, SQL, Python, статистике и визуализации.

Проект построен на [MkDocs](https://www.mkdocs.org/) и теме [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

## Содержание

- [Введение в аналитику и Google Таблицы](docs/sprint-01-analytics-google-sheets/index.md)
- [Основы SQL. Извлечение данных](docs/sprint-02-sql-extraction/index.md)
- [SQL. Обработка данных](docs/sprint-03-sql-processing/index.md)
- [SQL. Анализ данных и ad hoc задачи](docs/sprint-04-sql-adhoc/index.md)
- [Визуализация данных с помощью DataLens](docs/sprint-05-datalens/index.md)
- [Основы Python](docs/sprint-06-python-basics/index.md)
- [Python. Предобработка данных](docs/sprint-07-python-preprocessing/index.md)
- [Исследовательский анализ данных и визуализация с помощью Python](docs/sprint-08-python-eda/index.md)
- [Расчёт и визуализация бизнес-метрик и показателей](docs/sprint-09-business-metrics/index.md)
- [Формулировка и проверка гипотез. Статистический анализ данных](docs/sprint-10-statistics/index.md)
- [Анализ результатов A/B-тестирования с помощью Python](docs/sprint-11-ab-testing/index.md)

## Запуск локально

```bash
python -m venv .venv
```

Windows:

```powershell
.venv\\Scripts\\activate
```

Linux / macOS:

```bash
source .venv/bin/activate
```

Установить зависимости:

```bash
pip install -r requirements.txt
```

Запустить локальный сервер:

```bash
mkdocs serve
```

После этого открыть адрес, который покажет MkDocs в терминале, обычно `http://127.0.0.1:8000/`.

## GitHub Pages

Сайт собирается и публикуется автоматически при каждом `push` в ветку `main` с помощью GitHub Actions.

В настройках репозитория необходимо выбрать:

**Settings → Pages → Source → GitHub Actions**

После первого успешного запуска workflow GitHub Pages будет опубликован автоматически.

## Структура проекта

```text
analytics-wiki/
├── README.md
├── mkdocs.yml
├── requirements.txt
├── .gitignore
├── .github/
│   └── workflows/
│       └── deploy.yml
└── docs/
    ├── index.md
    ├── stylesheets/
    │   └── extra.css
    └── sprint-XX-.../
        ├── index.md
        └── *.md
```
