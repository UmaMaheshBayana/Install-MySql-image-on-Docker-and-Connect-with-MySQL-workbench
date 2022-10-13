# Install-MySql-image-on-Docker-and-Connect-with-MySQL-workbench


```
docker run -d --restart unless-stopped -p 3306:3306 --name mysql-new -e MYSQL_ROOT_PASSWORD=root mysql:5.7.34
````

Given permissions for User to connect from MYSQL Workbench

```
GRANT ALL PRIVILEGES ON *.* TO 'root'@'localhost' WITH GRANT OPTION;
````

```
CREATE USER 'root'@'%' IDENTIFIED BY '$some_pass';
````

```
GRANT ALL PRIVILEGES ON *.* TO 'root'@'%' WITH GRANT OPTION;
````
