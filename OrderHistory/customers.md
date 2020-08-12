```sql
CREATE TABLE customers (id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    -> full_name VARCHAR(50),
    -> username VARCHAR(50),
    -> email VARCHAR(50),
    -> no_hp INT(50),
    -> address VARCHAR(50));

// ganti no_hp jadi varchar

ALTER TABLE customers
    -> DROP COLUMN no_hp;

ALTER TABLE customers
    -> ADD no_hp VARCHAR(50);

//input info

INSERT INTO `customers` (`id`, `full_name`, `username`, `email`, `address`, `no_hp`) VALUES (NULL, "Christiana Yeo", "Chris", "chrisyeo.tr@gmail.com", "Jakarta Utara", "081261802823");
INSERT INTO `customers` (`id`, `full_name`, `username`, `email`, `address`, `no_hp`) VALUES (NULL, "David Winalda", "David", "davidwinalda94@gmail.com", "Jakarta Utara", "0813452587");
INSERT INTO `customers` (`id`, `full_name`, `username`, `email`, `address`, `no_hp`) VALUES (NULL, "Rumondang Tampubolon", "Mon", "rumondang@gmail.com", "Jakarta Utara", "0856613301");
INSERT INTO `customers` (`id`, `full_name`, `username`, `email`, `address`, `no_hp`) VALUES (NULL, "Ridho Abdul Majid", "Ridho", "ridho@gmail.com", "Bandung", "08564215235");
 INSERT INTO `customers` (`id`, `full_name`, `username`, `email`, `address`, `no_hp`) VALUES (NULL, "Budhi Arta", "Budhi", "budhi@gmail.com", "Bali", "087786452321");

```sql