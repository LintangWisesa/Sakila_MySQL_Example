![simplinnovation](https://4.bp.blogspot.com/-f7YxPyqHAzY/WJ6VnkvE0SI/AAAAAAAADTQ/0tDQPTrVrtMAFT-q-1-3ktUQT5Il9FGdQCLcB/s600/simpLINnovation1a.png)

# Install Sakila Database MySQL Example

#### 1. Download & extract it to your directory, e.g. *C:\data\db*. When you unpack the archive, it creates a directory named *sakila-db* that contains *sakila-schema.sql, sakila-data.sql, sakila.mwb & SampleSakila.png* files.

#### 2. Connect to the MySQL server using the mysql command-line client with the following command:

```shell
$ cd C:\Program Files\MySQL\MySQL Server 5.7\bin
$ mysql.exe --user=your.user.name --password=your.pass
```

#### 3. Execute the sakila-schema.sql script to create the database structure by using the following command:

```shell
mysql> SOURCE C:/data/db/sakila-db/sakila-schema.sql;
```

#### 4. Execute the sakila-data.sql script to populate the database structure with the following command:

```shell
mysql> SOURCE C:/data/db/sakila-db/sakila-data.sql;
```

#### 5. Confirm that the sample database is installed correctly. Execute the following statements:

```shell
mysql> show databases;
```
```shell
mysql> use sakila;
```
```shell
mysql> show tables;
```
```shell
mysql> select * from actor
```
#### 6. Here is the database design of Sakila Database:

![Sakila Database Design](https://raw.githubusercontent.com/LintangWisesa/Sakila_MySQL_Example/master/SampleSakila.png)

### More information [click here](https://dev.mysql.com/doc/sakila/en/sakila-introduction.html).
