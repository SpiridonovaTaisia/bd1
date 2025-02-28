1. Выберите из таблицы orders 3 самых дешевых заказа за все время. 
Данные нужно отсортировать в порядке убывания цены. Отмененные заказы не учитывать.

SELECT * FROM orders WHERE products_count>0 AND STATUS IN ('new', 'in_progress', 'delivery)
ORDER BY SUM DESC LIMIT 3;
![image](https://github.com/user-attachments/assets/8ed914c2-9e50-4970-8589-afa52b8cae41)
2. Выберите из таблицы orders 2 самых дорогих заказа за все время. Данные нужно отсортировать в порядке убывания цены. 
Отмененные заказы не учитывайте.

SELECT * FROM orders WHERE STATUS IN ('new', 'in_progress', 'delivery)
ORDER BY SUM DESC LIMIT 2;
![image](https://github.com/user-attachments/assets/ca296fa2-5fe7-4722-ba89-2eb265b661d5)
3. Добавьте в таблицу orders данные о новом заказе стоимостью 8000 рублей. В заказе 4 товара (products).

INSERT INTO orders (id, products, sum)
VALUE (6, 4, 8000);
![image](https://github.com/user-attachments/assets/5f53407a-f85d-439d-872a-3429395ed71e)
4. Добавьте в таблицу products новый товар — «VR-очки», стоимостью 70000 рублей в количестве (count) 2 штук.

INSERT INTO products (id, name, count, price)
VALUE (7, 'VR-очки', 2, 70000);
![image](https://github.com/user-attachments/assets/13f3009f-2e61-4fc8-9d00-1cf38d633f75)
5. В таблицу products внесли данные с ошибкой, вместо "PS5" в наименовании написали IMAC. Исправьте ошибку.
![image](https://github.com/user-attachments/assets/2fde4625-d460-414c-b21e-1afd2adc44d5)
