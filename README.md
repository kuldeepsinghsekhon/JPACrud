# JPACrud
Jpa EclipseLink Test Project having swing and  cli Front End  
This Project is for student training purpose only, In this i used EclipseLink JPA Implimentation and inserted 
few values in table name users. still i did not use auto table create. but later will use all.
mysql> use project
Database changed
mysql> show tables;
+-------------------+
| Tables_in_project |
+-------------------+
| customers         |
| users             |
+-------------------+
2 rows in set (0.03 sec)

mysql> show create table users;
+-------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Table | Create Table                                                                                                                                                                                                                                                                                                                                                                                                              |
+-------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| users | CREATE TABLE `users` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `email` varchar(80) NOT NULL,
  `name` varchar(32) NOT NULL,
  `password` varchar(32) NOT NULL,
  `activation` int(2) DEFAULT NULL,
  `activ_date` date DEFAULT NULL,
  `last_login` date DEFAULT NULL,
  `role` varchar(20) DEFAULT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `email` (`email`)
) ENGINE=InnoDB AUTO_INCREMENT=77 DEFAULT CHARSET=latin1 |
+-------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
1 row in set (0.11 sec)
Here is output of Cli Main.java

==============================
Please Enter  A Choice
==============================
 1. Insert User 
 2. Update User 
 3. Delete User 
 4. List All User 
 5. Search By  User Name 
 0. Exit 
4
===================================================================================================
| USERID| EMAIL                       | NAME                        | PASSWORD                    |
===================================================================================================
| 51    | sad                         | dsa                         | sad                         |
| 101   | fdgd                        | gfsgsfg                     | fdgfdgfdg                   |
| 102   | fdgd                        | gfsgsfg                     | fdgfdgfdg                   |
| 151   | kuldeep@mail.com            | kuldeep singh               | kssekhon                    |
| 152   | lucky@mail.com              | lucky                       | 123455                      |
===================================================================================================

==============================
Please Enter  A Choice
==============================
 1. Insert User 
 2. Update User 
 3. Delete User 
 4. List All User 
 5. Search By  User Name 
 0. Exit 
5
Enter user name of user
k
===================================================================================================
| USERID| EMAIL                       | NAME                        | PASSWORD                    |
===================================================================================================
| 151   | kuldeep@mail.com            | kuldeep singh               | kssekhon                    |
| 152   | lucky@mail.com              | lucky                       | 123455                      |
===================================================================================================
==============================
Please Enter  A Choice
==============================
 1. Insert User 
 2. Update User 
 3. Delete User 
 4. List All User 
 5. Search By  User Name 
 0. Exit 
2
Enter user ID of user
152
Enter user Email
lucky123@gmail.com
Enter user name
luckymartin
Enter user Password
martinjaa

==============================
Please Enter  A Choice
==============================
 1. Insert User 
 2. Update User 
 3. Delete User 
 4. List All User 
 5. Search By  User Name 
 0. Exit 
4
===================================================================================================
| USERID| EMAIL                       | NAME                        | PASSWORD                    |
===================================================================================================
| 51    | sad                         | dsa                         | sad                         |
| 101   | fdgd                        | gfsgsfg                     | fdgfdgfdg                   |
| 102   | fdgd                        | gfsgsfg                     | fdgfdgfdg                   |
| 151   | kuldeep@mail.com            | kuldeep singh               | kssekhon                    |
| 152   | lucky123@gmail.com          | luckymartin                 | martinjaa                   |
===================================================================================================
==============================
Please Enter  A Choice
==============================
 1. Insert User 
 2. Update User 
 3. Delete User 
 4. List All User 
 5. Search By  User Name 
 0. Exit 
3
Enter user ID of user
51

==============================
Please Enter  A Choice
==============================
 1. Insert User 
 2. Update User 
 3. Delete User 
 4. List All User 
 5. Search By  User Name 
 0. Exit 
4
===================================================================================================
| USERID| EMAIL                       | NAME                        | PASSWORD                    |
===================================================================================================
| 101   | fdgd                        | gfsgsfg                     | fdgfdgfdg                   |
| 102   | fdgd                        | gfsgsfg                     | fdgfdgfdg                   |
| 151   | kuldeep@mail.com            | kuldeep singh               | kssekhon                    |
| 152   | lucky123@gmail.com          | luckymartin                 | martinjaa                   |
===================================================================================================
