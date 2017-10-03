Tips to Shield Your WP Site by Rodrigo Donini (@donini on twitter)

Note created by Gregory Hammond (@devGregory on twitter, @gregoryhammond on github)

Proper config
Proper development / good practices
Update
Use [wpscan.org](https://wpscan.org/) or [wpvulndb.com](https://wpvulndb.com/) as a scanner / checker
Remove or change not to be admin (username) and with ID 1
Black access to user list
 - add to .htaccess
 - url pattern /?author=1
Use strong passwords
Increase security with hases
 - security-key
Two-step authentication (sms, qrcode, ping, google auth)
Used constants: wp, debug, debug_log, debug_display
Protect debug.log
- location: wp-content/debug.log
- chmod 600
<files debug.log>
order allow,deny

Expose version of WordPress
- remove version, or .htaccess deny from all\

Remove / block access:
/readme.html
/license.txt
/wp-config-sample.php
/wp-admin

Full path disclosure
- plugin (for WordPress) to change it, and remove wp_ from table name

Directory protection
protect wp-config.php - [https://codex.wordpress.org/Editing_wp-config.php](https://codex.wordpress.org/Editing_wp-config.php)
 -> if you move wp-config to another location it doesn't move back when updated
 
 disallow_file_edit vs disallow_edit_mods
 file_edit disables file changes in themes & plugins
 edit_mods disallow files changes & automatic updates
 
 Almost 60% of WordPress installs are outdated
 
 Plugins
 - Wordfence
 - Sucuri
 - Sitelock
 - iThemes Security
 
Don Security (created by speaker) - [https://github.com/donini/don-security](https://github.com/donini/don-security)

Good to change passwords after 6 months