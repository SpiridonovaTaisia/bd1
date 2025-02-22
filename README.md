1)Выберите из таблицы orders все заказы
SELECT * FROM orders;
![image](https://github.com/user-attachments/assets/97a891a2-d932-4e1b-b2a6-1e79ebda9e96)
2)Выберите из таблицы orders все заказы кроме новых. У новых заказов status равен "new". Использовать in
SELECT * FROM orders WHERE STATUS IN ('in_progress', 'cancelled', 'delivery');
![image](https://github.com/user-attachments/assets/00146861-7388-4e93-93ac-9798e349ef97)
3)Выберите из таблицы orders все новые и отмененные заказы. У отмененных заказов status равен "cancelled".
У новых заказов status равен "new".
SELECT * FROM orders WHERE STATUS IN ('cancelled', 'new');
![image](https://github.com/user-attachments/assets/a5dd5535-996d-4884-babf-c7fba4ba851f)
4)Выберите из таблицы orders все заказы содержащие более 3 товаров (products_count).
Вывести нужно только номер (id) и сумму (sum) заказа.
SELECT  id, sum FROM orders WHERE products_count > 3;
![image](https://github.com/user-attachments/assets/d8d95346-b495-449d-b13e-6b930d203bdf)
# bd1
