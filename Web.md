## Hydra
  hydra -l username -P passwordlist.txt -s PORT IP http-post-form 'referurl:postbody^user^&^password:Error message'

## Netcat listener
  nc -nlvp PORT

## ICO
  * Identify a website framework from its ICO
  * curl ICO | md5sum
  * [OWASP ICO](https://wiki.owasp.org/index.php/OWASP_favicon_database)
