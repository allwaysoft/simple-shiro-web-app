simple-shiro-web-app
====================

A simple proof-of-concept of Shiro authentication with Jetty and JDBC (MySQL) Realm.

## Prerequisites ##
- JDK 6
- Maven 3.0.3 or newer

## Configure MySQL database ##

Run the following commands:  
```
mysql -u root -p
create database shiro;  
grant all privileges on shiro.* to 'shiro'@'localhost' identified by '123qwe';
flush privileges;
```

Now, populate the database with the script provided: 
```
mysql -u root -p123qwe shiro < pop_db.sql
```

## Test ##

Run in Tomcat. Point your browser to _http://localhost:8080_
