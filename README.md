# php-5.6-with-magic-quotes
This project allows you to use magic_quotes_gpc with php-5.6 and php-7

I have re-implemented magic_quotes_gpc for PHP 5.6.34.

This patch allows you to run your very legacy code on a very modern version of PHP (up to PHP 7).

This way, you get advantage of all the recent modules (redis, memcache, elasticsearch, etc), security and performance enhancements while being able to run very outdated code.
With this patch, you can finally upgrade the Debian machine that you installed 15 years ago.

PHP 5.6.34 was picked, as this is the last stable version of PHP that supports mysql_connect().
mysql_* is a MySQL driver that was very popular 10 years ago;
If are using magic_quotes_gpc, you are probably using this mysql driver too.

I don't use this code, and probably nobody should ever do but I'm sure it's useful.

Arnaud.
