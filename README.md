# Проект Foodgram

**«Продуктовый помощник» — сайт, на котором можно публиковать рецепты, добавлять чужие рецепты в избранное и подписываться на публикации других авторов. Сервис «Список покупок» позволяет пользователям скачать список продуктов, которые нужно купить для приготовления выбранных блюд.**

### Запуск проекта локально:
  
Клонировать репозиторий и перейти в него:  
  
```  
git clone https://github.com/yankovskaya-ktr/foodgram-project-react.git
cd foodgram-project-react
``` 

Создать файл .env по шаблону .env.template:

```
cp .env.template .env
```
Запустить приложение:

``` 
docker-compose up
``` 
Провести миграции:

``` 
docker-compose exec web python manage.py migrate --noinput
``` 

Создать суперпользователя:

``` 
docker-compose exec web python manage.py createsuperuser
``` 

Импортировать данные в базу данных:  
  
```  
docker-compose exec web python manage.py import_data


### Автор: https://github.com/yankovskaya-ktr/