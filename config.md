# Mysql

```shell
# install mysql
sudo apt install mysql-server
# login in mysql as root with no password
sudo mysql -uroot -p
# mysql >
# create user account,foo is user name，123 is password,
CREATE USER foo@localhost IDENTIFIED BY '123';
# set or update user password
# method 1 if update current account password can just set password=...
SET PASSWORD FOR 'username'@'host' = PASSWORD('newpassword')
# method 2 user info in user table mysql db 
update mysql.user set password=password('新密码') where User="phplamp" and Host="localhost";
```

