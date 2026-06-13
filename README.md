# Deploy — @papaleshapro Landing

Однофайловый лендинг на GitHub Pages.

## Структура

```
deploy/
├── index.html          # Единственный файл лендинга
└── .publish-flag.json  # Флаг готовности к деплою
```

## Публикация

1. Запушить в ветку `main`
2. GitHub Action автоматически задеплоит папку `deploy/` на GitHub Pages
3. Сайт будет доступен по адресу: `https://<username>.github.io/<repo>/`

## Ручной деплой

Если нужно обновить без пуша — триггерни `workflow_dispatch` в Actions.

## Настройка (один раз)

1. Settings → Pages → Source: **GitHub Actions**
2. Первый пуш в `main` запустит деплой
