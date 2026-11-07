#🐾 Луна — блог годовалой девочки-голден ретривера на Flask. Анимированные SVG-иллюстрации, 9 статей, адаптивный дизайн.

# 🐾 Луна — блог золотистого ретривера

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-3.0-green?logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![License](https://img.shields.io/badge/License-MIT-pink)](LICENSE)

Веб-блог от лица годовалой девочки-голден ретривера по имени **Луна**.  
Милая, но полностью рабочая Flask-заготовка для учебного проекта или портфолио.

![Превью сайта](static/luna.svg)

---

## ✨ Что внутри

- 🏠 **4 страницы:** Главная, Записи, Обо мне, Написать мне
- 📖 **9 статей** от лица собаки — с юмором и в первом лице
- 🎨 **4 авторских SVG-иллюстрации** — все нарисованы вручную прямо в коде
- 🐕 **Анимация виляющего хвоста** через `<animateTransform>` — без JavaScript и CSS
- 💖 **Живые детали:** мячик подпрыгивает, сердечко парит, конверт покачивается
- 🎨 **Пастельная палитра** и адаптивная вёрстка (mobile-friendly)
- 🧩 **Jinja2-шаблоны** с общим `base.html` и наследованием блоков
- 📬 **Форма обратной связи** (демо, без бэкенда — `alert()` вместо отправки)

---

## 🚀 Быстрый старт

### 1. Клонируйте репозиторий
```bash
git clone https://github.com/ВАШ_ЛОГИН/luna-blog.git
cd luna-blog
```

### 2. Создайте виртуальное окружение
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Установите зависимости
```bash
pip install -r requirements.txt
```

### 4. Запустите приложение
```bash
python app.py
```

### 5. Откройте в браузере
```
http://127.0.0.1:5000
```

---

## 📁 Структура проекта

```
luna-blog/
├── app.py                  # Flask-приложение и список постов
├── requirements.txt        # Зависимости (Flask, gunicorn)
├── README.md
├── .gitignore
├── templates/
│   ├── base.html           # Общий шаблон (header + footer)
│   ├── index.html          # Главная
│   ├── posts.html          # Все записи
│   ├── about.html          # Обо мне
│   └── contact.html        # Написать Луне
└── static/
    ├── style.css           # Все стили
    ├── luna.svg            # Портрет для главной
    ├── posts.svg           # Луна с мячиком
    ├── about.svg           # Луна сидит
    └── contact.svg         # Луна с конвертом
```

---

## 🛠️ Технологии

| Что | Зачем |
|-----|-------|
| **Python 3.10+** | Язык |
| **Flask 3.0** | Веб-фреймворк |
| **Jinja2** | Шаблонизация (входит во Flask) |
| **HTML5 / CSS3** | Разметка и стили |
| **SVG + SMIL** | Иллюстрации с анимацией |

Никаких Node.js, сборщиков, фреймворков на фронте — только чистый Flask и браузер.

---

## 🎨 Как добавить новую статью

Откройте `app.py`, найдите список `POSTS` и добавьте элемент:

```python
{
    "id": 10,
    "emoji": "🍖",
    "color": "c-sand",
    "date": "20 мая 2026",
    "title": "Моя первая косточка",
    "excerpt": "Краткое описание в одну строку.",
    "body": "Полный текст статьи от лица Луны."
},
```

Доступные цвета карточек: `c-pink`, `c-sand`, `c-berry`, `c-mint`, `c-sky`, `c-sun`, `c-lavender`, `c-ice`.

---

## 🌍 Деплой

Сайт можно бесплатно опубликовать:

- **[PythonAnywhere](https://www.pythonanywhere.com/)** — проще всего, работает в браузере
- **[Render.com](https://render.com/)** — подключите GitHub-репозиторий, старт-команда `gunicorn app:app`
- **[Replit](https://replit.com/)** — для быстрого теста

Файл `requirements.txt` уже содержит всё нужное.

---

## 📜 Лицензия

Распространяется по лицензии **MIT**.  
Используйте, форкайте, вдохновляйтесь — Луна не против 🐶

---

## 💌 Обратная связь

Если проект пригодился — поставьте ⭐ звёздочку.  
Если нашли баг — создайте [issue](https://github.com/ВАШ_ЛОГИН/luna-blog/issues).

Сделано с любовью и печеньками 🦴
