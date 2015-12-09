# Set Up Postgresql on Cloud9 Online IDE

## Start Postgresql on Cloud9 

Type `sudo service postgresql start`

## Set Up User

A default Postgres installation has a user account with the following information: 

Username: `username`

Password: `password`

There are 2 problems to solve with the Cloud9 (C9) Postgres installation:

1. The Postgres on C9 doesn't have `password` as the password for the root user
2. The Postgres on C9 is encoded in ASCII instead of UTF8

To fix #1, do the following:

Type `sudo sudo -u postgres psql` into the console, which will bring you into the Postgres interactive terminal

Then, you type `ALTER USER postgres WITH PASSWORD 'password';`.  It should spit out `ALTER ROLE` if you did it right.

To fix #2, do the following: 

Copy and paste these commands into the Postgres interactive terminal one by one:

`UPDATE pg_database SET datistemplate = FALSE WHERE datname = 'template1';`

`DROP DATABASE template1;`

`CREATE DATABASE template1 WITH TEMPLATE = template0 ENCODING = 'UNICODE';`

`UPDATE pg_database SET datistemplate = TRUE WHERE datname = 'template1';`

`\c template1`

`VACUUM FREEZE;`

`UPDATE pg_database SET datallowconn = FALSE WHERE datname = 'template1';`

Once your done, just type `\q` to get out of the Postgres interactive terminal

## Set Up Rails Databases
 
Type `rake db:create:all` 
