# Cursor-Aim-Css-and-JavaScript-FrameWork

<h1> How To Use?</h1>

```bash
composer install
```

Buat database di Phpmyadmin dan ubah konfigurasi database di `application/config/database.php`.

```php
$active_group = 'default';
$query_builder = TRUE;

$db['default'] = array(
	'dsn'	=> '',
	'hostname' => 'localhost',
	'username' => 'root', // <- sesuaikan dengan username mysql
	'password' => '', // <- isi dengan password user mysql
	'database' => 'beritacoding', //<- sesuaikan nama database dengan yang kamu buat
	'dbdriver' => 'mysqli',
	'dbprefix' => '',
	'pconnect' => FALSE,
	'db_debug' => (ENVIRONMENT !== 'production'),
	'cache_on' => FALSE,
	'cachedir' => '',
	'char_set' => 'utf8',
	'dbcollat' => 'utf8_general_ci',
	'swap_pre' => '',
	'encrypt' => FALSE,
	'compress' => FALSE,
	'stricton' => FALSE,
	'failover' => array(),
	'save_queries' => TRUE
);
```
