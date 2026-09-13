# NEKO Construction

Сайт строительной компании NEKO Construction (Seattle, WA).
Статический сайт, публикуется через GitHub Pages.

## Структура

| Файл | Что |
|---|---|
| `index.html` | Главная |
| `service-areas.html` | Хаб зоны обслуживания |
| `seattle.html` … `everett.html` | Страницы городов |
| `media/` | Видео и кадры для hero |
| `sitemap.xml`, `robots.txt` | Для Google Search Console |

## Как обновлять

Страницы собираются скриптом из соседней папки проекта:

```bash
python3 build.py     # собирает в dist/
```

Затем содержимое `dist/` копируется сюда и коммитится.
Города правятся в `src/cities.py`.

## Осталось сделать

- номер лицензии WA L&I (искать `class="todo"`)
- email и часы работы
- реальные фотографии объектов вместо `<div class="slot">`
- подключить форму заявки к обработчику
- заменить `BASE_URL` в `build.py` на купленный домен
