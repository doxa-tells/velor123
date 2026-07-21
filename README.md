# VELOR Academy of Hospitality & Service

Сайт первой швейцарской академии гостеприимства и сервиса в Центральной Азии.

**Стек**: статичный single-file HTML + vanilla JS + inline CSS. Без сборки.

## Структура

```
.
├── index.html       # вся разметка, стили, скрипты, i18n
└── assets/          # фотографии и логотип
```

## Запуск локально

Открыть `index.html` в браузере — всё работает из коробки.

Или поднять простой локальный сервер:

```bash
python3 -m http.server 8000
# открыть http://localhost:8000
```

## Деплой

Статика — можно класть куда угодно: GitHub Pages, Netlify, Vercel, Cloudflare Pages, любой хостинг.

## SEO

- `robots.txt` и `sitemap.xml` лежат в корне — рассчитаны на домен `https://velor.academy`.
- Canonical, hreflang (`?lang=ru|kz|en`), Open Graph, Twitter Cards и JSON-LD (EducationalOrganization, WebSite, FAQPage) — в `<head>` `index.html`.
- После деплоя: добавить сайт в Google Search Console и Яндекс.Вебмастер, отправить sitemap, проверить разметку через validator.schema.org.
- При смене домена — заменить `velor.academy` в `index.html`, `robots.txt`, `sitemap.xml`.

## Админка

Раздел публикации новостей живёт по адресу `/index.html#admin`. Пароль задан в коде в константе `ADMIN_PASS` — поменять перед публикацией.

## Языки

RU / KZ / EN — переключатель в шапке. Переводы лежат в объекте `I18N` внутри `index.html`.

## Контакты

Заявки уходят на: `o.iksanova@ssd.team`
