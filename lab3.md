Создайте таблицу users с полем id типа INT и двумя текстовыми полями, которые будут хранить имя (first_name) и фамилию (last_name).
Длина имени и фамилии не превышает 50 символов.
Добавьте в таблицу трех пользователей: Дмитрия Иванова, Анатолия Белого и Дениса Давыдова.

CREATE TABLE users (id INT, first_name VARCHAR (50), last_name VARCHAR (50));
INSERT INTO users (id, first_name, last_name)
VALUE (1, 'Дмитрий', 'Иванов'),
(2, 'Анатолий', 'Белый'),
(3, 'Денис', 'Давыдов');
![image](https://github.com/user-attachments/assets/5b7036e5-d0e6-4971-b655-904454b47ec0)
![image](https://github.com/user-attachments/assets/975436f9-a8eb-4b61-ab49-5a82d9dcaf1f)

