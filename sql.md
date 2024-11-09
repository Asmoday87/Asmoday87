В качестве репрезентации опыта работы с SQL-запросами рассмотрим сайт Alikson.ru. В частности работа с профилем (добавление, удаление, обновление информации о пользователе)

**Цель:** продемонстрировать работу с INSERT, DELETE, UPDATE, SELECT

**Пояснение:** Все операции провожу над таблицей Profile, которая имеет следующие поля last_login, username, first_name, last_name, email, 
is_active, phone, date_of_birth.

_Добавляю пользователя:_
```SQL
INSERT INTO Profile (last_login, username, first_name, last_name, email, 
is_active, phone, date_of_birth)
values (NULL, 'volfgun_666@gmail.com', 'Семен', 'Коржов', 
'volfgun_666@gmail.com', TRUE, '+7-906-563-45-91', '1966-10-27')
```
_Обнавляю информацию о пользователе:_
```SQL
UPDATE Profile 
SET date_of_birth = '1999-09-26'
WHERE id = 10
```
_Удаление несокльких пользователей:_
```SQL
DELETE FROM Profile
WHERE ID > 5 AND ID < 8
```
_Вывод пользователей с почтовым ящиком @gmail.com:_
```SQL
SELECT *
FROM Profile
WHERE email LIKE '%@gmail.com'
```
