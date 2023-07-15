[Official Mass Assignment](https://laravel.com/docs/10.x/eloquent#mass-assignment)

Open **php artisan tinker**.

> Our User model have specified fillable and gaurded fields inside the model.
> _Make sure to restart the tinker and again start after doing any changes in codebase._

**We can use `User::ungaurded()` & `User::regard()` commands to bypass the fillable and gaurded properties.**

