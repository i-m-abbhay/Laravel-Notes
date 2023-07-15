We have a basic login/register facility up untill now which is provided by `breeze`. We want to give user the functionality to add an avatar.

1. At first We have to create a column to store the avatar field in the database.
2. We did that after creating a new migration.
3. Tinker -> A CL Application which is for interacting your application.
4. Tinker can help filling the avatar information for the existing users.
    > php artisan tinker _This will open a command line interface for our laravel app. You can run all sort of php commands in the CLI._

```php
$user = User::find(4);
$user->avatar = 'skdalkdhlk';
$user->save();
```

**There is another method**

```php
$user = User::find(12);
$user->update([
  'avatar' => 'aldaslkdaslj'
]);
```

> But The above method will not reflect the change in Database despite returning true.

### Here comes the yet another laravel functionality [mass assignment](MassAssignment.md) into the picture.