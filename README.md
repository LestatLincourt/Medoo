![](https://raw.githubusercontent.com/catfan/Medoo/develop/src/medoo-logo.png)

## [Medoo](http://medoo.in)

[![Total Downloads](https://poser.pugx.org/catfan/medoo/downloads)](https://packagist.org/packages/catfan/medoo)

[![Latest Stable Version](https://poser.pugx.org/catfan/medoo/v/stable)](https://packagist.org/packages/catfan/medoo)

[![License](https://poser.pugx.org/catfan/medoo/license)](https://packagist.org/packages/catfan/medoo)

> The Lightest PHP database framework to accelerate development

## Main Features

* **Lightweight** - 25KB around with only one file.

* **Easy** - Extremely easy to learn and use, friendly construction.

* **Powerful** - Support various common and complex SQL queries.


* **Security** - Prevent SQL injection.

* **Free** - Under MIT license, you can use it anywhere if you want.

## Get Started

### Install via composer

Add Medoo to composer.json configuration file.
```
$ composer require catfan/Medoo
```

And update the composer
```
$ composer update
```

```php
// If you installed via composer, just use this code to requrie autoloader on the top of your projects.
require 'vendor/autoload.php';

// Or if you just download the medoo.php into directory, require it with the correct path.
require_once 'medoo.php';

// Initialize
$database = new medoo([
    'database_type' => 'mysql',
    'database_name' => 'name',
    'server' => 'localhost',
    'username' => 'your_username',
    'password' => 'your_password',
    'charset' => 'utf8'
]);

// Enjoy
$database->insert('account', [
    'user_name' => 'foo',
    'email' => 'foo@bar.com',
    'age' => 25,
    'lang' => ['en', 'fr', 'jp', 'cn']
]);
```

## Contribution Guides

For most of time, Medoo is using develop branch for adding feature and fixing bug, and the branch will be merged into master branch while releasing a public version. For contribution, submit your code to the develop branch, and start a pull request into it.

On develop branch, each commits are started with `[fix]`, `[feature]` or `[update]` tag to indicate the change.

Keep it simple and keep it clear.

## License

Medoo is under the MIT license.

## Links

* Official website: [http://medoo.in](http://medoo.in)

* Documentation: [http://medoo.in/doc](http://medoo.in/doc)