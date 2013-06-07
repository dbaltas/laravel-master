laravel-master
==============

This is the default sample downloaded from laravel website.
It seems to work OK with paratest v0.4.4

After running

    composer update

version 0.4.4 of brianium/paratest is installed

```
 ~/projects/laravel-master (master)$ phpunit
PHPUnit 3.7.21 by Sebastian Bergmann.

Configuration read from /home/dbaltas/projects/laravel-master/phpunit.xml

.

Time: 0 seconds, Memory: 8.50Mb

OK (1 test, 1 assertion)
 ~/projects/laravel-master (master)$ vendor/bin/paratest

Running phpunit in 5 processes with /home/dbaltas/projects/laravel-master/vendor/bin/phpunit

Configuration read from /home/dbaltas/projects/laravel-master/phpunit.xml

.

Time: 0 seconds, Memory: 3.75Mb

OK (1 test, 1 assertion)
```


### NOTE:
Please note that when I require brianium/paratest `dev-master` of paratest

I get the following error when running 

     composer update

```
PHP Fatal error:  Class 'Patchwork\Utf8\Bootup' not found in /home/dbaltas/projects/laravel-master/bootstrap/autoload.php on line 46
PHP Stack trace:
PHP   1. {main}() /home/dbaltas/projects/laravel-master/artisan:0
PHP   2. require() /home/dbaltas/projects/laravel-master/artisan:16
Script php artisan optimize handling the post-update-cmd event returned with an error


                                                                                                                                               
  [RuntimeException]                                                                                                                           
  Error Output: PHP Fatal error:  Class 'Patchwork\Utf8\Bootup' not found in /home/dbaltas/projects/laravel-master/bootstrap/autoload.php on   
  line 46                                                                                                                                      
  PHP Stack trace:                                                                                                                             
  PHP   1. {main}() /home/dbaltas/projects/laravel-master/artisan:0                                                                            
  PHP   2. require() /home/dbaltas/projects/laravel-master/artisan:16                                                                          

```

