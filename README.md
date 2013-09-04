MyPython
========

Python programming practice

Mac OS setup mysql problems
====

mysql_config not found

```
export PATH=$PATH:/usr/local/mysql/bin
```

install python-mysqldb

- Downloaded mysql_python and unzipped it
- Installed mysql_python

```
python setup.py install
```

MySQL on OSX: Library not loaded: libmysqlclient.18.dylib

```
sudo ln -s /usr/local/mysql/lib/libmysqlclient.18.dylib /usr/lib/libmysqlclient.18.dylib
```

Mysql root password reset

```
$ mysql -u root
mysql> use mysql;
mysql> update user set password=PASSWORD("NEWPASSWORD") where User='root';
mysql> flush privileges;
mysql> quit
```
