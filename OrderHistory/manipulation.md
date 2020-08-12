```sql
SELECT * FROM customers;
SELECT * FROM products;

INSERT INTO `transactions` (`id_product`, `id_customer`) VALUES (3, 4);
INSERT INTO `transactions` (`id_product`, `id_customer`) VALUES (2, 1);
SELECT transactions.id, customers.id
    -> FROM transactions
    -> INNER JOIN customers ON transactions.id = customers.id
    -> INNER JOIN products ON transactions.id = products.id
    -> ;
SELECT transactions.id, products.id, customers.full_name, customers.email, products.product_name, products.price 
FROM transactions 
INNER JOIN customers ON transactions.id_customer = customers.id 
INNER JOIN products ON transactions.id_product = products.id;
