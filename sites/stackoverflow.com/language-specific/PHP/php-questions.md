###[Q] (PHP) What errors?
What do you mean by "not working"? Do you get any errors? Add [error reporting](//php.net/manual/function.error-reporting.php) at the top of your file(s): `ini_set("display_errors", 1); error_reporting(E_ALL);` and tell us what you get.

###[Q] (PHP) mysql_* API
[**Please don't use `mysql_*` functions in new code**](//stackoverflow.com/q/12859942)! They are no longer maintained [and are officially deprecated](//wiki.php.net/rfc/mysql_deprecation). See the [**red box**](//php.net/manual/function.mysql-connect.php)? Learn about [*prepared statements*](//en.wikipedia.org/wiki/Prepared_statement) instead, and use [PDO](//php.net/pdo) or [MySQLi](//php.net/mysqli) - [this article](//php.net/manual/mysqlinfo.api.choosing.php) can help you choose. If you go with PDO, [here is a good tutorial](http://wiki.hashphp.org/PDO_Tutorial_for_MySQL_Developers).

###[Q] (PHP) SQL Injection
[Your script is at risk for SQL Injection Attacks.](//stackoverflow.com/q/60174)
