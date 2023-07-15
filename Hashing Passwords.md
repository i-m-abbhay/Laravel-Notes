Laravel provides you with the global `bcrypt()` function to incrypt your password.
We can use Eloquent model and perform mutation to change our password from simple string to a hashed string.
You can checkout about mutator in Laravel's official Documentation.

> You have to create a protected function with the same name as the field name. And then the set part is the mutation. & the get part is accessor.

Inside the `app/Models/User.php` below function is responsible for hashing the password during saving into the database via User Model. It's a Mutator.

```php

protected function password(): Attribute

    {

        return Attribute::make(

            set: fn ($value) => bcrypt($value)

        );

    }

```

Similar to mutator there is also accessor. Checkout the official Documentation for more information.