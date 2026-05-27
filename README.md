# 💍 Юрий & Диана — свадебный сайт

## Структура
```
wedding/
├── index.html          — главная страница
├── styles.css          — все стили
├── netlify.toml        — настройки деплоя
├── assets/             — фото и иконки
└── fonts/              — кастомные шрифты
    ├── EvgeniaDeco.ttf  ✅ есть
    ├── PosteRetro.ttf   ✅ есть
    └── WonderGarden.ttf ⚠️ нужно добавить вручную
```

## ⚠️ Шрифт Wonder Garden

Этот шрифт недоступен для автоматической загрузки.  
Пока используется **Marck Script** (похожий кириллический скрипт, Google Fonts).

Чтобы подключить оригинальный Wonder Garden:
1. Скачай файл `WonderGarden Script.ttf` (у тебя должен быть, раз использовался в Figma)
2. Переименуй в `WonderGarden.ttf`
3. Положи в папку `fonts/`
4. Готово — CSS уже настроен, шрифт подхватится автоматически

## 📋 Форма анкеты гостя (Formspree)

1. Зайди на [formspree.io](https://formspree.io) → Sign Up (бесплатно)
2. Создай новую форму → получи ID вида `xabcdefg`
3. В `index.html` найди строку:
   ```
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
4. Замени `YOUR_FORM_ID` на свой ID
5. Ответы гостей будут приходить на email, с которым ты регистрировался

Лимит бесплатного тарифа: **50 отправок / месяц** (для свадьбы хватит).

## 🚀 Деплой на Netlify (бесплатно)

### Вариант 1 — перетащить папку (30 секунд)
1. Зайди на [app.netlify.com](https://app.netlify.com)
2. Перетащи папку `wedding/` прямо в браузер
3. Получишь URL вида `random-name.netlify.app`
4. Можно сразу переименовать: Site settings → Change site name

### Вариант 2 — через GitHub (с автообновлением)
```bash
cd /home/yuriy/VSCODE/wedding
git init
git add .
git commit -m "Wedding site initial"
gh repo create wedding --public --push
```
Затем в Netlify: Add new site → Import from Git → выбери репозиторий.

### Свой домен
В Netlify: Domain management → Add custom domain → следуй инструкции.

## 🗺️ Карта
В `index.html` кнопка "Открыть на карте" ведёт на Яндекс.Карты по адресу  
**г. Сызрань, Дамбовская 1** — можно заменить на Google Maps ссылку.

## 📞 Контакты координатора
Телефон и WhatsApp координатора Маши уже вставлены: **+7 (937) 060-55-14**.
