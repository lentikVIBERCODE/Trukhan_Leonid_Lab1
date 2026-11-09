# Лабораторная работа 1 — набор S31

Анализ снижения частоты успешных операций и три группы для кампании банка «Меридиан». Все данные синтетические.

## Запуск

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m playwright install chromium
jupyter lab
```

Из корня проекта выполните `01_analysis.ipynb` сверху вниз, затем `02_report.ipynb`. Сырые файлы находятся в `S31/`; промежуточные очищенные таблицы — в `results/`.

```bash
jupyter nbconvert --to webpdf --no-input --execute 02_report.ipynb --output report.pdf --WebPDFExporter.paginate=True
```

Для запуска выберите Python виртуального окружения. У первого ноутбука все результаты и графики сохранены; второй строит три графика и читает очищенные результаты первого.

## Сдаваемые файлы

- `01_analysis.ipynb` — аудит, очистка, исследование, правила отбора.
- `02_report.ipynb` — аналитическая записка.
- `report.pdf` — печатный отчёт.
- `cleaning_log.csv` — журнал решений.
- `campaign_list.csv` — 1924 клиента в трёх группах.

