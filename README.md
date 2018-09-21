## Laravel 5 example ##

**Laravel 5 example** provides fake data to seed your database table, as well as a clean install of Laravel 5. This fork was created to give students at [Linux Academy](https://linuxacademy.com) an easy application to launch when building a VPC from scratch on AWS.

### Installation ###

* `git clone https://github.com/christophelimpalair/laravel5-example application`
* `cd application`
* `curl -sS https://getcomposer.org/installer | php`
* `php composer.phar install`
* `php artisan key:generate`
* Setup database details in .env (RDS details if you're following the lesson)
* `php artisan migrate --seed` to create and populate tables. If this step fails, you have either misconfigured your .env database info, or your RDS security group configuration is not allowing EC2 instances to connect. Make sure you have the proper inbound and outbound rules.


### Database Seeding ###

To test application the database is seeding with users :

* Administrator : email = admin@test.com, password = admin
* User : email = user@test.com, password = redac