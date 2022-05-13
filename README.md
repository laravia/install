# install

## docker - sail
> use this 
<pre>
docker-compose.yml
</pre>

# testing

## env.testing
use testing .env
<pre>
cp .env .env.testing
</pre>

## testing
> for testing add one line to phpunit.xml

```xml
<testsuites>
    <testsuite name="Unit">
        <directory suffix="Test.php">./packages/</directory>
    </testsuite>
</testsuites>
```
