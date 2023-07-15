Instead of running raw SQL queries we can use something called the query building inside the DB facade.

```php
$users = DB::table('users')->where('id', 1)->get();
//There are more methods which we can chain in to create query such as
//->update(['field1','value1', 'field2','value2'])
//->delete()
dd($users);

```

_But you can see this doesn't seem to be that gamechanging. Hold on a minute my friend._
**There are other usefull methods to chain.**
`->value('email')`, `->find(1)` -> find uses key by default, `->chunk(100)` etc.

[[Eloquent ORM]] helps us to provide even a better method than this