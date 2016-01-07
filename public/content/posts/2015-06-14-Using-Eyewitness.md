---
published: false
---

## A New Post

#download Eyewitness

#create target list with EyeWitness pulling http targets from nmap scan
    ./EyeWitness.py /path/to/nmap/scan —createtargets
#run eyewitness
    ./EyeWitness.py -f <createtargetsfile.txt> -t 15
