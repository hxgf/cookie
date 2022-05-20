# Cookie

### PHP functions to handle cookie operations more easily.


# Installation
Easy install with composer:
```
composer require hxgf/cookie
```
```php
use Cookie\cookie;
require __DIR__ . '/vendor/autoload.php';
```

# Usage

## cookie::set($key, $value, $expiration_date)
Sets a cookie with a specific key for a specific amount of time.
```php
cookie::set(
  'user_name',
  'Buzz',  // can be a string or an array or whatever
  1461619625  // optional, in unix time format, default is time() + 31536000000
);
```

## cookie::get($key)
Returns the value of a specific cookie.
```php
echo cookie::get('user_name');  // Buzz
```

## cookie::delete($key)
Deletes a specific cookie.
```php
cookie::delete('user_name');
```
