# Cortex Lab — квиз-лендинг

Одностраничный сайт-квиз (чистый HTML/CSS/JS, без сборки).
Заявки уходят через Formspree, при сбое открывается почтовый клиент.

## Структура

- `index.html` — весь сайт
- `netlify.toml` — настройки деплоя на Netlify
- `.gitignore`

## Публикация на GitHub

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<ваш-логин>/<репозиторий>.git
git push -u origin main
```

## Деплой на Netlify

1. Netlify → **Add new site** → **Import an existing project** → выберите GitHub и этот репозиторий.
2. Параметры подтянутся из `netlify.toml` (Build command — пусто, Publish directory — `.`).
3. Нажмите **Deploy**. Дальше каждый `git push` в `main` публикуется автоматически.

## Что настраивается в коде

Блок `CFG` в `index.html` (в `<script>`): название компании, email,
адрес формы Formspree (`endpoint`), заголовки, вопросы квиза.

## Заявки на почту

Письма приходят на email, указанный в настройках формы на formspree.io.
Адрес нужно подтвердить по ссылке из письма Formspree.
