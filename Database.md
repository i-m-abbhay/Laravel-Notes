php [[artisan]] [[migrate]] -> this command will create the database as well as necessary table for you if there is a server running mysql on the defined configurations in [[EnvFile.md]].

Laravel picks the name of db defined in [[EnvFile.md]]. and fetch all the necessary details for connection in `/config/database.php` 
Sometimes there is some issue with some sql queries. Make sure to install [[dbal|dbal]].
