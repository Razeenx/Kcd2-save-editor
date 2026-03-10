# KCD2 Save Editor — PWA

Редактор сохранений **Kingdom Come: Deliverance II** в виде Progressive Web App.  
Работает в браузере, устанавливается на Android/iOS/Desktop как приложение.

## Деплой на GitHub Pages (5 минут, бесплатно)

### 1. Создать репозиторий

1. Зайти на [github.com](https://github.com) → **New repository**
2. Имя: `kcd2-editor` (или любое другое)
3. Тип: **Public** ← обязательно для бесплатного Pages
4. Нажать **Create repository**

### 2. Загрузить файлы

Перетащить все 5 файлов прямо в браузере на страницу репозитория:

```
index.html
manifest.json
sw.js
icon-192.png
icon-512.png
```

Или через Git:
```bash
git init
git add .
git commit -m "KCD2 Save Editor"
git remote add origin https://github.com/ВАШ_НИК/kcd2-editor.git
git push -u origin main
```

### 3. Включить GitHub Pages

1. В репозитории → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / `(root)`
4. Нажать **Save**

Через ~1 минуту сайт будет доступен по адресу:  
`https://ВАШ_НИК.github.io/kcd2-editor/`

### 4. Установить на телефон

1. Открыть ссылку в **Chrome на Android**
2. Подождать несколько секунд — появится баннер **«Установить как приложение»**
3. Нажать **УСТАНОВИТЬ**
4. Готово — иконка появится на рабочем столе

## Альтернативы GitHub Pages

| Хостинг | Бесплатно | HTTPS | Скорость деплоя |
|---------|-----------|-------|-----------------|
| [GitHub Pages](https://pages.github.com) | ✓ | ✓ | ~1 мин |
| [Netlify](https://netlify.com) | ✓ | ✓ | ~30 сек (drag & drop папку) |
| [Vercel](https://vercel.com) | ✓ | ✓ | ~30 сек |

**Netlify** — самый простой: просто перетащить папку `kcd2-editor/` на сайт netlify.com/drop

## Структура файлов

```
kcd2-editor/
├── index.html      — редактор (весь JS/CSS внутри)
├── manifest.json   — PWA манифест (имя, иконки, цвета)
├── sw.js           — service worker (кэш, офлайн)
├── icon-192.png    — иконка 192×192
└── icon-512.png    — иконка 512×512
```

## Как пользоваться

1. Найти файл сохранения на ПК:  
   `%LOCALAPPDATA%\Kingdome Come Deliverance II\Saved Games\`
2. Скопировать `.whs` файл на телефон (USB, облако)
3. Открыть редактор → выбрать файл
4. Изменить нужные параметры → **Сохранить файл**
5. Перенести изменённый файл обратно на ПК
