# LdapRecord-Laravel Example Project
Example Laravel project for [LdapRecord-Laravel](https://github.com/DirectoryTree/LdapRecord-Laravel) with the [Forum Systems Online LDAP Test Server](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/).

## Setup
 1. Clone the project
 2. Change in the project folder
 3. Run `composer install`
 4. Copy the `.env.example` to `.env`
 5. Setup the your database in the `.env` file
 6. Add these lines at the end of the `.env` file  
```
LDAP_LOGGING=true
LDAP_CONNECTION=default
LDAP_HOST=ldap.forumsys.com
LDAP_USERNAME=null
LDAP_PASSWORD=null
LDAP_PORT=389
LDAP_BASE_DN="dc=example,dc=com"
LDAP_TIMEOUT=5
LDAP_SSL=false
LDAP_TLS=false
```
 7. Run `php artisan key:generate`
 8. Run `php artisan migrate`
 9. Open site and login with username `einstein` and password `password` (Check [Online LDAP Test Server](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/) for more information of the Online LDAP Test Server)

## Thanks
  - [Steve Bauman](https://github.com/stevebauman) for [LdapRecord-Laravel](https://github.com/DirectoryTree/LdapRecord-Laravel)
  - [Forum Systems](https://www.forumsys.com/) for their [Online LDAP Test Server](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/)
  - [Conor](https://stackoverflow.com/users/6426405/conor) for [his answer on "cloning laravel project from github"](https://stackoverflow.com/a/39913449/2246865)
