php-encoding-test
=================

PHP encoding test from Kunststube: http://kunststube.net/frontback/

The config.php contains the DB login data:

define('_DB_HOST_', 'localhost');
define('_DB_NAME_', 'YOUR_DB_NAME');
define('_DB_USER_', 'YOUR_USER_NAME');
define('_DB_PASS_', 'YOUR_PASSWORD');


Create a utf-8 encoded table like so:

CREATE TABLE `texts` (
  `id` INT(11) unsigned NOT NULL AUTO_INCREMENT,
  `text` TEXT CHARACTER SET utf8,
  PRIMARY KEY (`id`)
) ENGINE=MyISAM DEFAULT CHARSET=utf8;