# 2018-05-21
## HTTPS on Wordpress sucks
Today I discovered that sometimes, when you add HTTPS to a Wordpress site, some plugins mess up with your redirections, getting to a loop... 😩
However, after strugling with this for a while, the solution was pretty simple. Just add this piece of code to `wp-config.php` file:
```php
$_SERVER["HTTPS"] = "on";
```
