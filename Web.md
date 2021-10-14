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
