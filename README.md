# madtesla
TO THE MOOOOOON

*** Please tell me who you are.

Run
```
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
git remote add origin https://github.com/thecryptosopher/madtesla.git
git status
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
git commit -am "commit message"
git push origin master
git pull origin master
```
 -->
# MADTESLA
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
## Development Setup 
### Automatic Setup
#### To build & configure the site run the following commands and follow instructions.
```
sudo add-apt-repository universe
sudo add-apt-repository multiverse
sudo add-apt-repository restricted
sudo apt update
sudo apt -y upgrade
```
### Manual Setup
#### Using Ubuntu
```
curl -sL https://deb.nodesource.com/setup_current.x | sudo -E bash -
sudo apt-get install -y nodejs
```
#### Using Debian, as root
curl -sL https://deb.nodesource.com/setup_current.x | bash -
apt-get install -y nodejs
To compile and install native addons from npm you may also need to install build tools:

#### use `sudo` on Ubuntu or run this as root on debian
```
sudo apt-get update
apt-get install -y build-essential
sudo apt-get install yarn

# Create the file repository configuration:
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'

# Import the repository signing key:
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -

# Update the package lists:
sudo apt-get update

# Install the latest version of PostgreSQL.
# If you want a specific version, use 'postgresql-12' or similar instead of 'postgresql':
sudo apt-get -y install postgresql
sudo apt-get install postgresql-13-postgis-3

sudo -u postgres -i
psql -d postgres < postgres.sql
psql -d crimson -U ruby
CREATE EXTENSION postgis;

```
### How to install:
```
yarn install

```
### How to run:
```
npm run start

```
### How to add a dependency : `<module-name>`
```
yarn add <module-name>
```
### How to update dependencies to the latest version:
```
sudo npm install -g npm-check-updates
ncu -u
npm update
npm install
```

from

    # TYPE DATABASE USER ADDRESS METHOD
    local  all      all          peer

to

    # TYPE DATABASE USER ADDRESS METHOD
    local  all      all          md5

- `peer` means it will trust the identity (authenticity) of UNIX user. So not asking for a password.

- `md5` means it will always ask for a password, and validate it after hashing with `MD5`.

- `trust` means it will never ask for a password, and always trust any connection.

You can, of course, also create more specific rules for a specific database or user, with some users having `peer` and others requiring passwords.

> After changing `pg_hba.conf` you'll need to restart PostgreSQL if it's running. E.g. `sudo service postgresql restart`



##### Steps to change/create default `postgres` user's password:

1. `trust` connection by adding in `pg_hba.conf` file

- `local all postgres trust`

2. Restart postgresql service

- `sudo service postgresql restart`

3. `psql -U postgres`

4. At the `postgres=#` prompt, change the user name `postgres` password:

- `ALTER USER postgres with password ‘new-password’;`

5. Revert the changes in `pg_hba.conf` file from `trust` to `md5` and restart `postgresql`.

##### pg_hba.conf file location

The file `pg_hba.conf` will most likely be at `/etc/postgresql/9.x/main/pg_hba.conf`
To check location of pg_hba.conf connect to postgres db using psql then type `SHOW hba_file;` command.

After change pg_hba.conf file, you can execute `SELECT pg_reload_conf();` or pg_ctl reload with superuser instead of restart postgresql service.

<sup>* [Source](http://stackoverflow.com/a/21889759/2945616) </sup>


## Sample Table
### protection(cloak, dagger) ⇒ <code>survival</code>

**Kind**: global functions

| Param | Type | Description |
| --- | --- | --- |
| cloak | <code>object</code> | Privacy gown |
| dagger | <code>object</code> | Security |

