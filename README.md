# php-roadmap
PHP Roadmap by Albert

#0. install php
Choices:
* Install XAMPP
* Install WAMP
* Install MAMP


# 1. basic variables
```php
<?php
$a = "Hello";
$b = "World";

echo $a;
```


# 2. array variables
```php
<?php
$a = ["Hello"," xxx ", "World"]

echo $a[2]; # the index starts with 0, so 0 is "Hello"

foreach ($a as $b => $c) {
   echo $a;
}
```



# 3. Associative array variables
```php
<?php

# you can make variables readable by giving them readable names
$brownie = [
   "name" => "Brownie",
   "age" => 10, # This is an integer
   "breed" => "Aspin"
]

echo $brownie['age']; # the index starts with 0, so 0 is "Hello"

foreach ($a as $b => $c) {
   echo $c;
}
```

# 4. SuperGlobals: $_GET and query strings
access the php file you made on the browser and append `?page=login&mode=show`

```php
<?php

echo $_GET['page']; # the index starts with 0, so 0 is "Hello"
echo "\n<br />\n"; # This is a line break

foreach ($_GET as $b => $c) {
   echo $c;
}
```



# 4. SuperGlobals: $_POST and html forms
access the php file you made on the browser and append `?page=login&mode=show`

```php
<?php

echo $_POST['username']; # the index starts with 0, so 0 is "Hello"
echo "\n<br />\n"; # This is a line break

foreach ($_POST as $b => $c) {
   echo $c;
}
```
