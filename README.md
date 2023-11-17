# laravel + orchid + laravia = amore

## how to install laravia (for server)

1.) install laravel (> 10)
> https://laravel.com/docs/10.x/installation
<pre>
    composer create-project laravel/laravel laravia
</pre>
1.1) config your app
<pre>
    cd laravia && nano .env
</pre>
1.2) run migrations
<pre>
    php artisan migrate
</pre>

2.) install orchid (with admin user)
> https://orchid.software/en/docs/installation/
<pre>
    composer require orchid/platform && php artisan orchid:install && php artisan orchid:admin admin admin@admin.com password
</pre>

3.) install laravia
> dev-main, without packagist.orgpackagist.org
Open your root composer.json
<pre>
    nano composer.json
</pre>
add laravia/heart to required the required section
<pre>
    "laravia/heart": "dev-main"
</pre>
Add the 'repositories' section to the bottom of the composer.json file, if it doesn't already exist.
<pre>
"laravia/heart": {
    "laravia": "core",
    "name": "heart",
    "type": "path",
    "url": "packages/laravia/heart"
},
</pre>
3.1) run composer
<pre>composer update</pre>

4.) login
open your browser and open the backend
<pre>
    localhost/admin/login
    user: admin@admin.com
    password: password
</pre>
