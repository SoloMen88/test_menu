# test_menu
Тестовое задание для АпТрейдер (UpTrader)      


## Приложение для отрисовки меню с помощью templatetag

### Содержание:
+ [Краткое описание](#краткое-описание)
+ [Полезные ссылки](#полезные-ссылки)
+ [Requirements](#requirements)
+ [Сборка и запуск проекта](#сборка-и-запуск)        




### Краткое описание:
Простое Django приложение для отрисовки древовидного меню, реализованное через templatetag. Меню и его элементы создаются и редактируются в админ панели Django. С помощью тега {% draw_menu 'menu_name' %} меню можно расположить на любой странице приложения.


## Стек
* Python
* Django
* SQLite3 



### Сборка и запуск:
! Для корректного отображения меню при запуске следует сначала создать его а так-же добавить в него элементы в админ панели Django.
```bash
git clone git@github.com:SoloMen88/test_menu.git
cd test_menu
python -m venv venv
source venv/Scripts/activate
pip install -r requirements.txt
cd test_menu/
python manage.py migrate
python manage.py runserver
```

После запуска проекта главная страница доступна по URL: http://localhost:8000/menu/?main_menu
Админка доступна по URL: http://localhost:8000/admin/