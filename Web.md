## Hydra
  hydra -l username -P passwordlist.txt -s PORT IP http-post-form 'referurl:postbody^user^&^password:Error message'

## Netcat listener
  nc -nlvp PORT

## ICO
  Get the framework of a website
  curl ICO | md5sum
  https://wiki.owasp.org/index.php/OWASP_favicon_database
