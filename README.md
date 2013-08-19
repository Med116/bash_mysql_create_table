bash_mysql_create_table
=======================
\n
A simple bash script that prompts user to enter column names, then goes through and asks for the column definition, then echos the full SQL \n query, then asks if you want to run it. \n

To Run this shell script, copy this file into where you keep your bash scripts, somewhere like ~/bin will do, thats where I keep mine.\n
\n
It takes one argumemt, the table name. \n
\n
Here is sample input/outut to craeate a 'members' table with the columns 'first_name', 'last_name', 'email_address': \n
\n
[shell user]$ create_table members \n
What column names do you want for the  table? (enter as space delimited)
first_name last_name email_address
define first_name :ie: INT(11) or VARCHAR(256)
VARCHAR(50)
define last_name :ie: INT(11) or VARCHAR(256)
varchar(100)
define email_address :ie: INT(11) or VARCHAR(256)
VARCHAR(120)
Do you want to run this query? y/n
CREATE TABLE members (id INT(11) PRIMARY KEY AUTO_INCREMENT,  first_name VARCHAR(50) , last_name varchar(100) , email_address VARCHAR(120) );
========================================
y
What is your mysql username?

[omitted]
What is your mysql database name?

[omitted]
Running Query:
        ++++++++++++++++++++++++++++++++++++++++
Schema for 'members'  will print if your query works after entering [omitted]'s mysql password.


Enter password:
Field   Type    Null    Key     Default Extra
id      int(11) NO      PRI     NULL    auto_increment
first_name      varchar(50)     YES             NULL
last_name       varchar(100)    YES             NULL
email_address   varchar(120)    YES             NULL
++++++++++++++++++++++++++++++++++++++++
