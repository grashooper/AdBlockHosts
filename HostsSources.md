## AdAway's default hosts sources

The following host sources are default in AdAway and thus supported by the author (see https://github.com/dschuermann/ad-away/wiki/HostsSources#what-are-the-criteria-to-make-a-hosts-source-default-in-adaway)

| URL     | SSL     | Description  | License |
| ------- | ------- | ------------ | ------- |
| https://adaway.org/hosts.txt | Y | Special hosts file for AdAway containing mobile ad provider | CC Attribution 3.0 |
| https://hosts-file.net/ad_servers.txt | Y | hpHosts | Allowed AdAway project to use it as default |
| https://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext | Y | Yoyos Hosts file | [MCRAE GENERAL PUBLIC LICENSE (version 4.r53)](https://pgl.yoyo.org/license/) |


## Other hosts sources

**WARNING: Using the following sources could kill cats, i.e., these sources are not officially supported.**

| URL     | SSL     | Description  | License |
| ------- | ------- | ------------ | ------- |
| http://winhelp2002.mvps.org/hosts.txt | N | MVPS HOSTS File, not available via SSL! | CC Attribution-NonCommercial-ShareAlike 3.0 |
| http://sysctl.org/cameleon/hosts | N | Some false positives (audiogalaxy) | Unknown |
| http://rlwpx.free.fr/WPFF/hosts.htm | N | Different available hosts files. Available as zip or 7z | Unknown |
| http://someonewhocares.org/hosts/hosts | Y (own cert) | Includes not only ad servers | Include URL |
| http://www.malwaredomainlist.com/hostslist/hosts.txt | ? | Malware list | Unknown |
| http://www.hostsfile.org/Downloads/hosts.txt or http://securemecca.com/Downloads/hosts.txt | ? | | Unknown |
| http://adblock.gjtech.net/?format=unix-hosts | N | Common US ad servers and farms | CC Attribution 3.0 |
| https://jansal.googlecode.com/svn/trunk/adblock/hosts | Y | | Unknown |
| https://sites.google.com/site/logroid/files/hosts.txt?attredirects=0 | Y | Japanese blocklist | Unknown |
| http://optimate.dl.sourceforge.net/project/adzhosts/HOSTS.txt | N | http://sourceforge.net/projects/adzhosts/ | Unknown |
| http://hosts.eladkarako.com/hosts.txt | N |  | Unknown |
| https://github.com/StevenBlack/hosts/raw/master/hosts | Y | https://github.com/StevenBlack/hosts | Unknown |
| https://github.com/yous/YousList/raw/master/hosts.txt | Y | https://github.com/yous/YousList | CC Attribution 4.0 International License |

## What are the criteria to make a hosts source default in AdAway?

* They should only block advertisement or analytic providers (for example http://sysctl.org/cameleon/hosts also blocks "shock sites", thus it is not included in AdAway)
* Hosts sources are potential security issues. The corresponding website of the hosts source should look "legit"
* The hosts sources have to be available directly as plain text. AdAway can not use zipped sources
* Malware blocking hosts sources are not included, because they would add too many entries
* Default hosts sources should not include redirection entries

If your hosts source complies with these requirements, open a [new Issue](https://github.com/dschuermann/ad-away/issues/new) and ask for inclusion!

## Censorship Circumvention

**WARNING: Only use these sources if you can't reach Google, Facebook, etc. from your country, because of DNS blocking!**

**If you want to use redirection rules from these Hosts Sources you have to explicitly allow redirection rules in the preferences of AdAway!**

| URL     | SSL     | Description  | License |
| ------- | ------- | ------------ | ------- |
| https://smarthosts.googlecode.com/svn/trunk/mobile_devices/hosts | Y |  | Unknown |
| https://veryhost.googlecode.com/files/android.txt | Y |  | Unknown |
| https://hostsx.googlecode.com/svn/trunk/hosts | Y |  | Unknown |

## Hosts file generator
| URL     | SSL     | Description  | License |
| ------- | ------- | ------------ | ------- |
| https://hostsaway.appspot.com/ | Y | Generate your own hosts source | CC0 |
| http://unblocksit.es/ | Y | Choose specific sites to unblock |  |