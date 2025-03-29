1)Выберите из таблицы orders 4 самых дорогих заказов за всё время.
Данные нужно отсортировать в порядке убывания цены.
Отмененные заказы не учитывайте.

SELECT * FROM orders WHERE STATUS IN ('new', 'in_progress', 'delivery') ORDER BY SUM DESC LIMIT 4;

![image](https://github.com/user-attachments/assets/9e1c14d7-0fd8-45a7-bde8-a02b498fc76c)

2) Выберите из таблицы products название и цены четырех самых дешевых товаров, которые есть на складе.

SELECT NAME, price from products WHERE COUNT>0 LIMIT 4;

![image](https://github.com/user-attachments/assets/997449e6-383a-4ce6-b821-77aff3f0c3cd)

3) Выберите из таблицы orders три последних заказа (по дате date) стоимостью от 3200 рублей и выше.
Данные отсортируйте по дате в обратном порядке.

SELECT * FROM orders WHERE SUM>=3200 ORDER BY DATE DESC LIMIT 3;

![image](https://github.com/user-attachments/assets/d0ec4f7b-ea11-4197-b5be-0628c77731de)

4) Создайте данную таблицу:

CREATE TABLE products (id INT, NAME VARCHAR (50), COUNT INT, price INT);
INSERT INTO products (id, NAME, COUNT, price)
VALUE (1, 'Стиральная машина', 5, 10000),
(2, 'Холодильник', 0, 10000),
(3, 'Микроволновка', 3, 4000),
(4, 'Пылесос', 2, 4500),
(5, 'Вентилятор', 0, 700),
(6, 'Телевизор', 7, 31740),
(7, 'Тостер', 2, 2500),
(8, 'Принтер', 4, 3000),
(9, 'Активные колонки', 1, 2900),
(10, 'Ноутбук', 4, 36990),
(11, 'Посудомоечная машина', 0, 17800),
(12, 'Видеорегистратор', 23, 4000),
(13, 'Смартфон', 8, 12300),
(14, 'Флешка', 4, 1400),
(15, 'Блендер', 0, 5500),
(16, 'Газовая плита', 5, 11900),
(17, 'Клавиатура', 3, 1800);

![image](https://github.com/user-attachments/assets/c82c180f-f94c-467b-8d67-745f8bb23030)

5) Из этой таблицы сделать выборку на основе задания: Сайт выводит товары по 5 штук. Выберите из таблицы products товары, которые пользователи увидят на 3 странице каталога при сортировке в порядке возрастания цены (price).

SELECT * FROM products ORDER BY price LIMIT 5 OFFSET 10;

![image](https://github.com/user-attachments/assets/dba2d832-abc0-44a8-bf81-ab45de48ffb4)


