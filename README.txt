You will need to make some changes to civicrm.settings.php. Ignore the usual guidance text for the cache settings and use something like these:

define( 'CIVICRM_DB_CACHE_CLASS', 'Redis' );
define( 'CIVICRM_DB_CACHE_HOST', 'localhost' ); // Add your redis server address
define( 'CIVICRM_DB_CACHE_PORT', portnumber ); // Add server's port
define( 'CIVICRM_DB_CACHE_PASSWORD', 'Server Password' ); // If your redis server needs a password, add it here.
define( 'CIVICRM_DB_CACHE_TIMEOUT', 3600 ); // Add your own choice here
