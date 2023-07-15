Go into `/bootstrap/cache` directory inside your root directory.

## Configuration Caching in Laravel

> in the php artisan we have `config` related command.
> if we run the `php artisan config:cache` command there will be a new file inside your `bootstrap/cache`. It is responsible for reading and storing all the necessary details of each and every file which was inside config for faster performance.

_Whenever you change something in `.env` (Make sure to add quotes if your string consists spaces.). We have to run `php artisan config:cache` again_

> `config:clear` removes the config cache