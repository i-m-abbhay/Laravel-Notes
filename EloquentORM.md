You can also use Eloquent ORM to perform query and this is a breeze. You can use the Model of the table to perform eloquent model.

```php
use App\Models\User;
// $user = User::create([
//   'name'=> 'Abhay',
//   'email'=> 'asdhbdh@gmail.com',
//   'password'=> 'password',
// ])

$user = User::where('id', 5)->first(); // In order to update the user you first have to get the user.
// we can also use ->find(5)
$user->update ([
  'email' => 'abc@iitism.ac.in'
]);

```

### The power of Eloquent

It has some amazing features such as seed, factories & policies that we will be learning in a moment.

> From the Model you can control the Table attributes and control the keys and other features such as increment of id and timestamp.