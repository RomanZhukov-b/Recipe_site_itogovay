# Проект “Сайт рецептов” на Django

[Проект развернут тут!](https://andybook.pythonanywhere.com/)

## Установка
1. Клонируйте репозиторий на ваше устройство:

    ```bash
    git clone https://github.com/RomanZhukov-b/Recipe_site_itogovay?tab=readme-ov-file
    ```

2. Установите зависимости:

    ```bash
    pip install -r requirements.txt
    ```

3. Создайте базу данных MySQL и настройте соединение с базой данных в файле settings.py:

    ```python
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.mysql',
            'NAME': 'database_name',
            'USER': 'username',
            'PASSWORD': 'password',
            'HOST': 'localhost',
            'PORT': '3306',
        }
    }
   ```
   
   Или можете раскомментировать следующие строки для работы с sqlite3 (и удалить строки ниже до блока `# Password validation`):
   ```python
   DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
         'NAME': BASE_DIR / 'db.sqlite3',
     }
   }
   ```
   
4. Примените миграции базы данных:

    ```bash
    python manage.py migrate
    ```

5. Для создания суперпользователя:

    ```bash
    python manage.py createsuperuser
    ```

6. Запустите сервер разработки Django:

    ```bash
    python manage.py runserver
    ```

7. Откройте ваш веб-браузер и перейдите по адресу http://localhost:8000/, чтобы начать использование приложения.

## Функции

- Регистрация и аутентификация пользователей
- Просмотр главной страницы с 5 случайными рецептами кратко
- Просмотр подробной информации о рецепте
- Добавление, редактирование и удаление рецептов
- Возможность добавления изображения для рецепта
- Категоризация рецептов

## Технологии

- Python
- Django - фреймворк для разработки веб-приложений
- MySQL - СУБД для хранения данных
- JavaScript - для добавления интерактивности и динамического поведения
- HTML/CSS - для создания пользовательского интерфейса



