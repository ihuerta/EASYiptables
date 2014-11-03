#EASYiptables 
#####Version 0.1

Descrption
----------
EASYiptables is a script written in Perl to simplify the use of iptables & options.

* Version 0.1 currently DROPS certain ports found open in Metasploitable 2.0.

- Intended to be used in Kali Linux or Metasploitable

##### This script uses the following system command lines
```
iptables -F
iptables -A INPUT -p tcp --match multiport --dport [HUGE LIST OF PORTS HERE] -j DROP
iptables-save
iptables -L -v -n --line-numbers

```

** LATER VERSIONS WILL OFFER WHICH PORTS YOU WANT TO DROP, ACCEPT, OR FORWARD


Version History

- 0.1 | initial release
