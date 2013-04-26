MyPython
========

Python programming practice

Mac OS setup mysql
====
mysql_config not found

    export PATH=$PATH:/usr/local/mysql/bin

install python-mysqldb

    Downloaded mysql_python and unzipped it
    Installed mysql_python using python setup.py install
    Tested it in an interactive session python, import _mysql
    
MySQL on OSX: Library not loaded: libmysqlclient.18.dylib

    sudo ln -s /usr/local/mysql/lib/libmysqlclient.18.dylib /usr/lib/libmysqlclient.18.dylib
