###[Q] What errors?
What does it mean "not working"? Do you get any errors? Add [error reporting](http://php.net/manual/en/function.error-reporting.php) at the top of your file(s): `ini_set("display_errors", 1); error_reporting(E_ALL);` and tell us what you get.

###[Q] mysql_* API
[**Please, don't use `mysql_*` functions in new code**](http://$SITEURL$/q/12859942). They are no longer maintained [and are officially deprecated](https://wiki.php.net/rfc/mysql_deprecation). See the [**red box**](http://php.net/manual/en/function.mysql-connect.php)? Learn about [*prepared statements*](http://en.wikipedia.org/wiki/Prepared_statement) instead, and use [PDO](http://php.net/pdo) or [MySQLi](http://php.net/mysqli).

###[Q] SQL Injection
[Your script is at risk for SQL Injection Attacks.](http://stackoverflow.com/q/60174)

###[Q] Parsing html with regex
[Please don't try to parse HTML with regex. Use a html-parse instead](http://stackoverflow.com/a/1732454/3933332)
