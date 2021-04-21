# Docker Environment for WordPress

- Wordpress installation goes into the ./src folder
- MySQL server is run on mysql:3306 and the setup is within ./env/mysql.env

### If WP prompts for FTP access

If WordPress asks you for the FTP access you need to add this to your wp-config.php

```
/** Allow Direct Updating Without FTP */
define('FS_METHOD', 'direct');

/* That's all, stop editing! Happy publishing. */
```
