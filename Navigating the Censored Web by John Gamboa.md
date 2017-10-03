Navigating the Censored Web by John Gamboa (@jgamboa on twitter)

Notes by Gregory Hammond (@devGregory on twitter, @gregoryhammond on github)

Slides available at [https://jpgamboa.com/wcto.pptx](https://jpgamboa.com/wcto.pptx)

You are not operating on a level playing field
Some countries have forced [data localization](https://en.wikipedia.org/wiki/Data_localization)
/wp-login.php is a ripe location

DNS poisoning
If have SSL site is likely to be blocked outright

Designing around censorship
- plugin communicate with external services (services that aren't your own website)
- hosting overseas or in-country
- test at [geopeeker.com](https://geopeeker.com/)
- PHP 7 is a must
- external ad services & API's
- consider global CDN's

Blocked check
China: [greatfire.org](https://en.greatfire.org/analyzer)
Iran: [https://www.comparitech.com/privacy-security-tools/blockediniran/](https://www.comparitech.com/privacy-security-tools/blockediniran/)
Russia: [https://reestr.rublacklist.net/](https://reestr.rublacklist.net/)

If want to be unblock
- check if recourse is available
- move to new server
- in-country or overseas
- may be noisy neighbours
- block may be domain or IP based
- may be nothing