# E-Commerce
An E-commerce Web Application with Admin Panel
          
# Install this project on your system

**You will need Apache-Tomcat server to run this project on your system**

-then create the following mysql tables


desc users;

+----------+-------------+------+-----+---------+----------------+

| Field    | Type        | Null | Key | Default | Extra          |

+----------+-------------+------+-----+---------+----------------+

| userId   | int(11)     | NO   | PRI | NULL    | auto_increment |

| email    | varchar(50) | YES  |     | NULL    |                |

| password | varchar(50) | YES  |     | NULL    |                |

| name     | varchar(50) | YES  |     | NULL    |                |

+----------+-------------+------+-----+---------+----------------+



desc sellers;

+----------+-------------+------+-----+---------+----------------+

| Field    | Type        | Null | Key | Default | Extra          |

+----------+-------------+------+-----+---------+----------------+

| id       | int(11)     | NO   | PRI | NULL    | auto_increment |

| name     | varchar(50) | YES  |     | NULL    |                |

| email    | varchar(50) | YES  |     | NULL    |                |

| password | varchar(50) | YES  |     | NULL    |                |

+----------+-------------+------+-----+---------+----------------+



desc products;

+-----------------------+-------------+------+-----+---------+----------------+

| Field                 | Type        | Null | Key | Default | Extra          |

+-----------------------+-------------+------+-----+---------+----------------+

| productId             | int(11)     | NO   | PRI | NULL    | auto_increment |

| productName           | varchar(50) | YES  |     | NULL    |                |

| productDescription    | varchar(50) | YES  |     | NULL    |                |

| productGender         | varchar(50) | YES  |     | NULL    |                |

| productCategory       | varchar(50) | YES  |     | NULL    |                |

| productQuantitySmall  | int(11)     | YES  |     | NULL    |                |

| productQuantityMedium | int(11)     | YES  |     | NULL    |                |

| productQuantityLarge  | int(11)     | YES  |     | NULL    |                |

| productSoldBy         | varchar(50) | YES  |     | NULL    |                |

| productPrice          | int(11)     | YES  |     | NULL    |                |

| productDiscount       | int(11)     | YES  |     | NULL    |                |

+-----------------------+-------------+------+-----+---------+----------------+



desc cart;

+-----------+-------------+------+-----+---------+-------+

| Field     | Type        | Null | Key | Default | Extra |

+-----------+-------------+------+-----+---------+-------+

| userEmail | varchar(50) | YES  |     | NULL    |       |

| productId | int(11)     | YES  | MUL | NULL    |       |

| size      | varchar(50) | YES  |     | NULL    |       |

+-----------+-------------+------+-----+---------+-------+
