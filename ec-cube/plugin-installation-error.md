# プラグインインストールエラー

```
In ExceptionConverter.php line 101:

    An exception occurred in the driver: SQLSTATE[HY000] [2002] php_network_getaddresses: getaddrinfo for db failed: nodename nor servname provided, or not known

In Exception.php line 28:  
    SQLSTATE[HY000] [2002] php_network_getaddresses: getaddrinfo for db failed: nodename nor servname provided, or not known  

In Driver.php line 33:

    SQLSTATE[HY000] [2002] php_network_getaddresses: getaddrinfo for db failed: nodename nor servname provided, or not known  

In Driver.php line 33:

    PDO::__construct(): php_network_getaddresses: getaddrinfo for db failed: nodename nor servname provided, or not known
```

インストールのときだけhostを`127.0.0.1`にしたらいけた

```
DATABASE_URL=mysql://db_user:db_password@db:3306/eccube
#DATABASE_URL=mysql://db_user:db_password@127.0.0.1:3306/eccube
```