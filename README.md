# Docker Environment for WordPress

- Wordpress installation goes into the `./src` folder
- MySQL server is run on `localhost:3306` and the setup is within `./env/mysql.env`

```
/** MySQL hostname */
define( 'DB_HOST', 'mysql' );
```

- Run `docker-compose up` to bring the environment up
- Run `docker-compose down` to shut down the environment

### If WP prompts for FTP access

If WordPress asks you for the FTP access you need to add this to your wp-config.php

```
/** Allow Direct Updating Without FTP */
define('FS_METHOD', 'direct');

/* That's all, stop editing! Happy publishing. */
```
