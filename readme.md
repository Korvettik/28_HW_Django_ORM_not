### Домашка 28

В этом задании мы углубляемся в различные методы работы с моделями и данными.

Для объявлений, категорий и пользователей реализован принцип CRUD.

Локации могут создаваться при создании нового пользователя.

В объявления можно загрузить картинки и отобразить их.

Для объявлений и пользователей реализована пагинация и сортировка. Сортировка также реализована и для категорий
(используется атрибут `orderong`).

Также в проекте функционирует админ-панель со всеми используемыми моделями.
___
Для запуска контейнера и наполнения базы необходимо в терминале набрать следующие команды:
```
docker-compose up -d
./manage.py migrate
./manage.py loaddata fixtures/ad.json fixtures/category.json fixtures/location.json fixtures/user.json
```