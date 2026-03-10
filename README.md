# KCD2 Save Editor — PWA

Редактор сохранений **Kingdom Come: Deliverance II** в виде Progressive Web App.  
Работает в браузере, устанавливается на Android/iOS/Desktop как приложение.

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
