We can run raw sql queries with something called **DB facade**.

```php

<?php
use Illuminate\Support\Facades\DB;
use Illuminate\Support\Facades\Route;
use App\Http\Controllers\ProfileController;

Route::get('/', function () {
// fetch all users
// $users = DB::select("select * from users where email=?", ['abhay.tiwari.er@gmail.com']);
// dd($users);

//create an user
// $user = DB::insert('insert into users (name, email, password) values (?,?,?)', ['Abhay', '20je0018@me.iitism.ac.in', 'password']);
// dd($user);

//updating user
// $user = DB::update("update users set email='abc@bitfumes.com' where id=2");
// dd($user);

//deleting user
// $user = DB::delete("delete from users where id=2");
// dd($user);

return view('welcome');

});

```

Sometimes running query through this might be a cumbersome method. That's why [[QueryBuilder]] came into the pictute. 