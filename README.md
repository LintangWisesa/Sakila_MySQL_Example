# Install Sakila Database MySQL Example

1. Download & extract it to your directory, e.g. **C:\data\db**. When you unpack the archive, it creates a directory named *sakila-db* that contains *sakila-schema.sql, sakila-data.sql, sakila.mwb & SampleSakila.png* files.

1. Connect to the MySQL server using the mysql command-line client with the following command:
```
$ cd C:\Program Files\MySQL\MySQL Server 5.7\bin
$ mysql.exe --user=your.user.name --password=your.pass
```

1. Execute the sakila-schema.sql script to create the database structure by using the following command:
```
mysql> SOURCE C:/data/db/sakila-db/sakila-schema.sql;
```

1. Execute the sakila-data.sql script to populate the database structure with the following command:
```
mysql> SOURCE C:/data/db/sakila-db/sakila-data.sql;
```

1. Confirm that the sample database is installed correctly. Execute the following statements. You should see output similar to that shown here.
```
mysql> show databases;
mysql> use sakila;
mysql> show tables;
mysql> select * from actor
```
1. Here is the database design of Sakila Database:
![Sakila Database Design](https://raw.githubusercontent.com/LintangWisesa/Sakila_MySQL_Example/master/SampleSakila.png)

### More information [click here](https://dev.mysql.com/doc/sakila/en/sakila-introduction.html).
