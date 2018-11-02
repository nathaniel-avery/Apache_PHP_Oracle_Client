# Apache_PHP_Oracle_Client
This project attempts to build a container running apache and php with the oracle instant client.  Apache and PHP are fairly common to find on legacy web front ends, and in a lot of those enviornments, they may need to connect to an Oracle database back end.  This POC tries to understand what it takes to make a container with those components talk to a database.  For simplicity, I inetend to use second container running Oracle as the target.

![apache_php_instantclient](https://user-images.githubusercontent.com/31746795/47942141-473f7780-dec7-11e8-9b81-38f2a1dbc4a8.png)
