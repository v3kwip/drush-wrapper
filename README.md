Drush Wrapper
====

```php
$drush = (new Drush())
  ->setDocRoot('/var/www/')
  ->setUri('http://drupal.example/')
  ->debug(true)
  ->command('user-password', 'username')
    ->param('password', 'new_password')
;

$json = $drush->execute();
```
