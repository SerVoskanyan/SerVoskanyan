# Portfolio v2 — A/B preview setup

## Что уже готово

| Версия | Где смотреть |
|--------|----------------|
| **README v1** (текущий) | https://github.com/SerVoskanyan |
| **README v2** (новый) | https://github.com/SerVoskanyan/SerVoskanyan/blob/main/README.v2.md |
| **Лендинг v1** | https://servoskanyan.github.io/My-cases/ |
| **Лендинг v2** (код) | https://github.com/SerVoskanyan/SerVoskanyan/tree/portfolio-v2 |

## Шаг 1 — Включить preview лендинга v2

1. Откройте **Settings → Pages** в репо `SerVoskanyan/SerVoskanyan`
2. **Build and deployment → Source:** выберите **GitHub Actions**
3. После этого workflow `Deploy portfolio v2 preview` задеплоит ветку `portfolio-v2`

Preview URL: **https://servoskanyan.github.io/SerVoskanyan/**

> Для корневого URL `https://servoskanyan.github.io/` нужен отдельный репо (шаг 2).

## Шаг 2 — Корневой URL (SerVoskanyan.github.io)

1. Создайте публичный репо: https://github.com/new?name=SerVoskanyan.github.io
2. Выполните из папки `landing-site`:

```bash
cd landing-site
git push -u origin main
```

3. **Settings → Pages → Source:** branch `main`, folder `/ (root)`

Готовый URL: **https://servoskanyan.github.io/**

## Шаг 3 — Выбрать победителя

- README: заменить `README.md` содержимым из `README.v2.md`
- Лендинг: обновить CTA в README на финальный URL
