### Install The passport
```SH
    $ cd /project/root
    $ composer require laravel/passport
```

### Run Migration and Install Passport Auth
    
```SH
    $ php artisan migrate
    $php artisan passport:install
```

### Make the AuthController
```SH
    php artisan make:controller Api\AuthController
```
