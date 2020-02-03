# Описание

Проект представляет собой блог для создания постов и тегов, между которыми реализовано отношение many-to-many.

После авторизации в роли админа станет доступно создание, редактирование и удаление постов и тегов. 
Реализован поиск по заголовкам и телу постов, есть пагинация. 

# Дополнительная информация

Используется CBV и миксины. 
В БД уникальность поста определяется его slug'ом, для этого решена проблема его уникальности. 

Для визуализации подключен Bootstrap 4 и кастомные CSS-стили. 


## Сборка и запуск

```bash
git clone https://github.com/cepjant/blog.git
cd blog
pip install virtualenv
python3.7 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```
