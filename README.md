# nginx-config-hacks
a personal repo of hacks i use to make nginx configs a tiny bit easier to manage

# structure
* root of this repo is /etc/nginx
* includes site configs in ./sites
* includes snippets in ./snippets
* also includes ./httpd if you're proxying to apache (which lives in /etc/httpd instead)
* some bash scripts in ./bin (which lives in ~/bin)

# credits / links / resources
* thanks to https://serversforhackers.com/c/nginx-php-in-subdirectory for the only config posted on the internet that actually works when hosting php apps in a subdirectory
* most other configs are either copied from or based on arch linux's package defaults or from the wiki

# looking for prototypical configs?
* sites/connectzaatari.conf = simple http one-pager, with optional assets
* sites/koken.conf = koken (uses snippets for everything)
* sites/trwnh.com = base site running pure html (intentionally doesn't include snippets/php.conf)
  * .../known = proxy pass to apache
  * .../portfolio = redirect to subdomain
  * .../october = php in subdirectory
