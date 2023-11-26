# RSUE_HACK_26.11.23
Установка
Для запуска данного приложения вам потребуется установить Django для Python. Вы можете сделать это, выполнив следующую команду в терминале:

bash
Copy code
pip install django
Запуск Приложения
Перейдите в директорию, где расположен файл manage.py.
Выполните команду:
bash
Copy code
python manage.py runserver
Откройте браузер и перейдите по адресу, который будет указан в терминале после выполнения команды runserver.
Миграция Базы Данных
Для переноса новых моделей в базу данных выполните следующие шаги:

Находясь в директории с файлом manage.py, выполните команду:
bash
Copy code
python manage.py makemigrations
После создания файлов миграции, выполните команду:
bash
Copy code
python manage.py migrate
Структура Проекта
Основной бэкэнд проекта разделен на следующие папки:

UsersPreferedDates: Хранит выбранные пользователем на сайте даты.
UsersQuery: Содержит SQL-запросы, используемые в проекте.
BurnOutMarkUps: В этой папке находятся файлы с функциями, связанными с гипотезами.
BurnOutAlgorithm: В этой папке находится конечный файл с результирующей функцией.
Примечание: Используемая база данных - db.sqlite3, а hahaton.db использовалась в качестве прототипа.

Запуск Проекта
Файл main.py содержит запуск основной функции, в которую передаются аргументы в виде других функций. Каждая из этих функций возвращает множества, необходимые для анализа.

