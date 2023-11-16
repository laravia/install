# first steps
0.) install composer
<pre>
https://getcomposer.org/download/
</pre>

# install laravia (for server)
1.) install laravel (> 10)
<pre>
composer create-project laravel/laravel laravia
</pre>

2.) go to directory "laravia"
<pre>cd laravia</pre>

3.) copy default .env.example
<pre>cp .env.example .env</pre>

4.) configurate your custom .env
> you need a database connection
<pre>nano .env</pre>

5.) run migrate
<pre>php artisan migrate</pre>

6.) install laravia/heart
> **dev-main** until first real laravia release
<pre>
    composer require laravia/heart:dev-main -n && composer config repositories.laravia/heart vcs https://github.com/laravia/heart
</pre>
