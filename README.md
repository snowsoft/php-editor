PHP editor extension for laravel-admin based on code-mirror
======

[DEMO](http://demo.laravel-admin.org/code-mirror/php) (Login using `admin/admin`)

## Installation 

```bash
composer require snowsoft/php-editor

php artisan vendor:publish --tag=laravel-admin-code-mirror
```

## Configuration

In the `extensions` section of the `config/admin.php` file, add some configuration that belongs to this extension.
```php

    'extensions' => [

        'php-editor' => [
        
            //Set to false if you want to disable this extension
            'enable' => true,
            
            // Editor configuration
            'config' => [
                
            ]
        ]
    ]

```

The configuration of the editor can be found in  [CodeMirror Documentation](https://codemirror.net/)

## Usage 

Use it in the form:
```php
$form->php('code');
```

Set height
```php
$form->php('code')->height(500);
```

 

License
------------
Licensed under [The MIT License (MIT)](LICENSE).
