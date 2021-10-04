# MySQL Workbench MariaDB compatibility patch

A patch that enables building MySQL Workbench from source code when using MariaDB development libraries on Debian. Tested on clean Debian 11 installation.

More on this topic: https://www.marekrost.cz/getting-mysql-workbench-to-work-on-debian-11

## How to apply
Example code:
```
wget https://dev.mysql.com/get/Downloads/MySQLGUITools/mysql-workbench-community-8.0.26-src.tar.gz
tar -xzf mysql-workbench-community-8.0.26-src.tar.gz
cd mysql-workbench-community-8.0.26-src
wget https://raw.githubusercontent.com/marekrost/mysql-workbench-debian-patch/main/mariadb-compat.patch
patch -p0 < mariadb-compat.patch
```
