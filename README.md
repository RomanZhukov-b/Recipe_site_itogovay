# Проект “Сайт рецептов” на Django

[Сайт рецептов находиться тут!](https://andybook.pythonanywhere.com/)

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




