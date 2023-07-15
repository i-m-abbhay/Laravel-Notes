It always starts with `.env` file. You can find `/config` directory in the root folder & there all the necessary configurations can be found.


> Laravel uses a global function `env(Key, default value)` in the php file to get the values from `.env` file.


_reading from this file again and again is not good for performance of our app. Hence laravel uses Caching to deal with this._