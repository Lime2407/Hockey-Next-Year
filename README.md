# NHL: предсказание успешности команды в следующем сезоне

**Автор:** Железкр Артём Андреевич aazhelezko@edu.hse.ru 
**Дата:** 12.10.2026
**Дата сбора данных:** 10.10.2026  

**Источник данных:** Scrape This Site — Hockey Teams, https://www.scrapethissite.com/pages/forms/ (24 страницы, 582 строки, сезоны 1990–2011, 2004 отсутствует).

**Использованные инструменты:** Python, pandas, numpy, scikit-learn, matplotlib; Claude (каюсь, он мне помогал разобраться с некоторыми заданиями и немного помог с scraper, редактировал текст, делал его читабельным и красивым).

## Состав
- `nhl_next_season.ipynb` — ноутбук с выполненными ячейками и ответами;
- `data/hockey_raw.csv` — исходная таблица с 9 требуемыми столбцами;
- `scrape_hockey.py` — собственный скрапер (запуск: `python scrape_hockey.py`);
- `data/hockey_teams_all_24_pages.csv` — готовая выгрузка (+ `source_page`), резерв и сверка.

## Воспроизведение
`pip install pandas numpy scikit-learn matplotlib` `requests beautifulsoup4` (для сбора; при `RUN_SCRAPE = True` ноутбук сам скачает сайт и впишет дату сбора), затем выполнить ноутбук сверху вниз. `RANDOM_STATE = 42`.
