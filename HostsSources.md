## Hosts file sources

| URL     | SSL     | Description  | License | Default in AdAway |
| ------- | ------- | ------------ | ------- | ----------------- |
| http://adaway.sufficientlysecure.org/hosts.txt | Y (own cert) | Special hosts file for AdAway containing mobile ad provider | CC Attribution | Y |
| http://winhelp2002.mvps.org/hosts.txt | N | MVPS HOSTS File | CC Attribution-NonCommercial-ShareAlike | Y |
| http://hosts-file.net/ad_servers.asp | N | hpHosts | Allowed AdAway project to use it as default | Y |
| http://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext | Y (with error) | Yoyos Hosts file | Unknown | Y |
| http://sysctl.org/cameleon/hosts | N | Some false positives (audiogalaxy) | Unknown | N |
| http://rlwpx.free.fr/WPFF/hosts.htm | N | Different available hosts files. Available as zip or 7z | Unknown | N |
| http://someonewhocares.org/hosts/hosts | Y (own cert) | Includes not only ad servers | Include URL | N |
| http://www.malwaredomainlist.com/hostslist/hosts.txt | ? | Malware list | Unknown | N |
| http://www.hostsfile.org/Downloads/hosts.txt or http://securemecca.com/Downloads/hosts.txt | ? | | Unknown | N |
| http://adblock.gjtech.net/?format=hostfile | ? |  | Unknown | N |
| https://jansal.googlecode.com/svn/trunk/adblock/hosts | Y | | Unknown | N |
| https://sites.google.com/site/logroid/files/hosts.txt?attredirects=0 | Y | Japanese blocklist | Unknown | N |
| http://optimate.dl.sourceforge.net/project/adzhosts/HOSTS.txt | N | http://sourceforge.net/projects/adzhosts/ | Unknown | N |

## What are the criteria to make a hosts source default in AdAway?

* They should only block Advertisments or Analytic Providers (for example http://sysctl.org/cameleon/hosts also blocks "shock sites", thus it is not included in AdAway)
* Hosts sources are potential security issues. The corresponding website of the hosts source should look "legit"
* The hosts sources have to be available directly as plain text. AdAway can not use zipped sources
* Malware blocking hosts sources are not included, because they would add too many entries
* Default hosts sources should not include redirection entries

## Redirection lists

**If you want to use redirection rules from these Hosts Sources you have to explicitly allow redirection rules in the preferences of AdAway!**

| URL     | SSL     | Description  | License | Default in AdAway |
| ------- | ------- | ------------ | ------- | ----------------- |
| https://smarthosts.googlecode.com/svn/trunk/mobile_devices/hosts | Y | Chinese hosts file to workaround blocked domains, Contains many redirection rules, not a blocklist | Unknown | N |
| https://veryhost.googlecode.com/files/android.txt | Y | Chinese hosts file to workaround blocked domains, Contains many redirection rules, not a blocklist | Unknown | N |
| https://hostsx.googlecode.com/svn/trunk/hosts | Y | Chinese hosts file to workaround blocked domains, Contains many redirection rules, also a blocklist | Unknown | N |

## Hosts file generator
| URL     | SSL     | Description  | License |
| ------- | ------- | ------------ | ------- |
| https://hostsaway.appspot.com/ | Y | Generate your own hosts source | CC0 |