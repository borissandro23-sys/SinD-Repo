# SinD — репозиторий для Sileo

Публичный APT-репозиторий для rootless-пакетов Dopamine.

## Адрес репозитория

После включения GitHub Pages добавь в Sileo:

`https://borissandro23-sys.github.io/SinD-Repo/`

## Как опубликовать пакет

1. Собери rootless-пакет `.deb` для архитектуры `iphoneos-arm64`.
2. Загрузи файл в папку `debs/` этого репозитория.
3. Открой вкладку **Actions** и запусти workflow **Update Sileo repository** (или дождись автоматического запуска после загрузки файла).
4. После успешного выполнения обнови источники в Sileo.

Workflow автоматически создаёт `Packages`, `Packages.gz` и `Release`.

## Включение GitHub Pages

В GitHub открой **Settings → Pages**:
- **Source:** Deploy from a branch
- **Branch:** `main`
- **Folder:** `/ (root)`

Сохрани настройки. Первое развёртывание Pages может занять несколько минут.

## Важно

- Репозиторий рассчитан на rootless-пакеты для Dopamine.
- Не загружай сюда rootful-пакеты.
- Публикуй только пакеты, которые ты имеешь право распространять.
