# php-roadmap
PHP Roadmap by Albert

#0. install php
Choices:
* Install XAMPP
* Install WAMP
* Install MAMP
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



# 3. associate array variables
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
   echo $a;
}
```

# 4. SuperGlobals: $_GET
access the php file you made on the browser and append `?page=login&mode=show`

```php
<?php
$a = ["Hello"," xxx ", "World"]

echo $a[2]; # the index starts with 0, so 0 is "Hello"

foreach ($a as $b => $c) {
   echo $a;
}
```
