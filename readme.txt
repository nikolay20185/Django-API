Авторизация с токеном через POSTMAN
POST auth/users/ - создание пользователя (Введите в formdata username, password)
POST api/auth/token/login/ - получение токена (Введите в formdata username, password)

В Headers добавьте Authorization,в его поле пропишите Token ваш токен
Теперь можно выполнять запросы как авторизованный пользователь

Корзина
api/carts/ - содержимое корзины
api/carts/add/ - Body/raw укажите в формате json строки product_id и количество quantity: { "product_id":1 "quantity":1}

api/carts/clear/ - Body/raw полное очищение корзины

api/carts/{id}/remove/ - Body/raw удаление  продукта из корзины по id продукта

api/carts/{id}/update_quantity/ - Body/raw изменение количества продукта из корзины по id продукта,
укажите в формате json строки количество на которое вы хотите изменить {"quantity": 2} 

Авторизация обычная с использованием api rest framework
/auth/users/ - создание пользователя
/simple-auth/login/ - авторизация

Админка - /admin/
Сначало надо создать суперюзера через терминал python manage.py createsuperuser

Swagger - /swagger/