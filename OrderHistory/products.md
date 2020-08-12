```sql
CREATE TABLE products (id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    -> product_name VARCHAR(50),
    -> price INT(50),
    -> stock INT(50));
SHOW tables;

INSERT INTO `products` (`id`, `product_name`, `price`, `stock`) VALUES (NULL, "Shoes", 258000, 30);
INSERT INTO `products` (`id`, `product_name`, `price`, `stock`) VALUES (NULL, "Hats",
159000, 50);
INSERT INTO `products` (`id`, `product_name`, `price`, `stock`) VALUES (NULL, "Jewelry", 1258000, 10);
INSERT INTO `products` (`id`, `product_name`, `price`, `stock`) VALUES (NULL, "Shirts", 315000, 60);
INSERT INTO `products` (`id`, `product_name`, `price`, `stock`) VALUES (NULL, "Socks", 48000, 100);
SELECT * FROM products;

```sql