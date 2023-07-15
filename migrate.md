Migrations are like version control for your [[Database]], allowing your team to define and share the application's [[database schema]] definition. If you have ever had to tell a teammate to manually add a column to their local database schema after pulling in your changes from source control, you've faced the problem that database migrations solve.

```shell
php artisan migrate
```

**It was not running in my case due to some compatibility issue with mariaDB version. But I've found a way to run raw SQL queries for the time being.**

_Laravel records all of the tables it has created during migration in a table named "migration" in our database. That means you cannot change anything by changing a migration file Laravel has already executed because it is not going to touch that file again._

![C:\Users\ASUS\Desktop\LaravelFreeCodeCamp\freeCodeGram\image.png](file:///c%3A/Users/ASUS/Desktop/LaravelFreeCodeCamp/freeCodeGram/image.png)
migrate
	[[migrate:fresh]] Drop all tables and re-run all migrations
	[[migrate:install]] Create the migration repository
	[[migrate:refresh]] Reset and re-run all migrations
	[[migrate:reset]] Rollback all database migrations
	[[migrate:rollback]] Rollback the last database migration
	[[migrate:status]] Show the status of each migration

