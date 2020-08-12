```sql

CREATE TABLE transactions (id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    -> id_product int NOT NULL,
    -> id_customer Int NOT NULL,
    -> FOREIGN KEY (id_product) REFERENCES products(id),
    -> FOREIGN KEY (id_customer) REFERENCES customers(id));

```sql