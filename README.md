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

# 5. Session: session_start()
create a single-user login page with username and password on variable, and session_start() to access $_SESSION superglobal

# 6. Login with a hardcoded password
Create a working login form that verifies the username and the password of the user

```php
<?php
function login($username, $password) {
   if ($username !== 'admin') {
      return false;
   }
   if ($password !== 'Pikachu0123') {
      return false;
   }
   return true;
}

login($_POST['username'], $_POST['password']);
?>
<form method='post'>
<input name='username' type='text' />
<input name='password' type='text' /> 
<button type='submit'>Submit</button>
</form>
```

Test case #1
1. Try with incorrect username and incorrect password
2. Expected: Invalid login

Test case #2
1. Try with correct username but wrong password
2. Expected: Invalid login

Test case #3
1. Try with incorrect username but correct password
2. Expected: Invalid login


Test case #4
1. Try with correct username and correct username
2. Expected: Redirects to login successful page, and visiting the login page redirects to login succesful page

Excercises:
1. change the type of the password field to "password" so the texts you type isn't visible
2. change the text of the button to "Login" so it is more accurate
3. change the function name "login" to something else (e.g. "loginAsAdmin()")

# 6. Study MySQL outside PHP
Install MySQL server on your computer and install a MySQL client
Study how to:
  * create a database,
  * create table
  * insert rows
  * update row
  * select row
  * delete roww
  * create a user table with username and password columns

# 7. Connect PHP to MySQL
Create a test script connect.php to test the mysql

```php
<?php
$username = 'localhost';
$username = 'username';
$password = 'password';
$port = '3306';
$database = 'my_database_name_replace_me';
$connection = mysqli_connect($host, $username, $password, $database, $port);

if (!mysqli_connect_errno()) {
    echo "Connected";
}
else {
   echo 'Error: ' . mysqli_connect_error());
}
?>
```

8. Select and list using PHP
9. Create dynamic pages using query string and select
