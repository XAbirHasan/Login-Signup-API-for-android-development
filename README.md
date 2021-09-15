All credit goes to [@VishnuSivadasVS](https://github.com/VishnuSivadasVS)  check out his work.

# LogIn and SignUp API using php with encryption.
A secure PHP API to manage login and signup operations. This API protects from attacks like SQL injunction and XSS. Also have password encryption. You can chnage anyting you want.

## How to use the API?
First of all download the files DataBase.php and DataBaseConfig.php. Place it in your project folder. Go to the DataBaseConfig.php file and change the details to your database details. Now add the file DataBase.php to your project file by requiring it.
```
require "DataBase.php";
```
Simply create an object for the class DataBase.
```
$db = new DataBase();
```
Call the dbConnect() and it will return a boolean value which shows whether the database connection is success of not. 
```
$db->dbConnect();
```
Inside the current file check the condition for database connection. If it is true proceed with the rest. Check this sample code.
```
require "DataBase.php";
$db = new DataBase();
if ($db->dbConnect()) {
    //Database connection is success.
}
else{
    //Database connection is failed.
}
```
Now that the connection is success you can call the login and the signup functions. Use the object of the class DataBase and call the functions.

### Calling Login Function
Call the logIn() with the object and pass the tablename, email and password as its arguments. Changes required as your database and need.
```
$db->logIn($tablename, $email, $password);
```

### Calling Signup Function
Call the signUp() with the object and pass tablename, name, phone, password and email as its arguments. hanges required as your database and need.
```
$db->signUp($tablename, $name, $phone, $password, $email);
```

Feel free to modify in this code.

## Authors

* **XAbirHasan**

Check out my other works [@XAbirHasan](https://github.com/XAbirHasan)

All credit goes to [@VishnuSivadasVS](https://github.com/VishnuSivadasVS)  check out his work.
