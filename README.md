# lems
LEARN Event Management System


## Installation

- Install git
-- apt-get install git-all  

- Clone the repository

- Install Dependencies

-- Install Composer
```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('SHA384', 'composer-setup.php') === '55d6ead61b29c7bdee5cccfb50076874187bd9f21f65d8991d46ec5cc90518f447387fb9f76ebae1fbbacf329e583e30') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```

-- Install Composer Globally (optional)

```
mv composer.phar /usr/local/bin/composer
```

-- Install Dependencies
```
composer install
```

-- Migrations

Create a database with name lemsdb, if not present.

```
create database lemsdb;
```

Run migrations, 
--- for ion_auth

```
run `/application/sql/ion_auth.sql` for ion_auth migrations, (user tables, etc)
```