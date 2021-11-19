## Hydra
  hydra -l username -P passwordlist.txt -s PORT IP http-post-form 'referurl:postbody^user^&^password:Error message'

## Netcat listener
  nc -nlvp PORT
  

## ICO
  * Identify a website framework from its ICO
  * curl ICO | md5sum
  * [OWASP ICO](https://wiki.owasp.org/index.php/OWASP_favicon_database)


## Gobuster
  * gobuster dir -u URL -w Wordlist(seclists/discovery/common is a good list) 

## Uploads
  * .phtml can bypass upload filters if the admin did not implement a proper upload check(Must be a php application)
  * [Wordpress uploads](https://www.hacknos.com/wordpress-shell-upload/)
  * If you have access to a wordpress administrator panel it is possible to upload a reverse shell via upload themes. The url schema is:
  * http(s)://IP/wp-content/uploads/year/day/filename

## XSS
* When testing payloads for XSS you can close the tag Hello <p div="name-return">Name Goes here</p>
* <p div="name-return"> </p>insert XSS payload. Example payload = "</p><cript>alert('XSS?');</cript>"
