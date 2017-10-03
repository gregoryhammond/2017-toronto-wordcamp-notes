Optimizing for High Traffic by Ian Forrest (@ianforr on twitter)

Slides available at [https://wordcamp2017.ianforrest.me/#/](https://wordcamp2017.ianforrest.me/#/)

Note created by Gregory Hammond (@devGregory on twitter, @gregoryhammond on github)

Why?
- faster
- better
- cheaper

1) Upgrade to PHP 7.1
- 50% improvement over 5.6
- can use php codesniffer & php comptability to check comptability

Caching
- plugins: wp rocket, total cache, super cache, comet cache
varnish for relatively static (user facing)
- grace period - if database goes down

WordPress transients
- [https://codex.wordpress.org/Transients_API](https://codex.wordpress.org/Transients_API)
- not optimal for caching data (slow)
- plugins exist

Spam / Attacks
- keep everything updated
- serve it to fewer people
- ban spammers -> use fail2ban or Wordfence

.htaccess
- nginx (alternative)

wp-cron
- schedule tasks in the future
- disable wp-cron in wp-config
- use [wp-cli](http://wp-cli.org/)

rest api
- logo performance good

AWS
- s3 - store file uploads - wp offload s3 (plugin)
- [cloudfront](https://aws.amazon.com/cloudfront/details/) - cdn

Load balancing
- scale - need multiple servers
- best if sessions are not sticky
- wordpress stores sessions in database
- avoid use of $_SESSION
- get wp-admin to get on one servers

Cache for longer than your update frequency
How do you know it's working? - use [newrelic](https://newrelic.com/)

If going to load test, then test on origin IP (make sure to tell your hosting company so they know so they don't block or stop your server)