# Common Problems with Solutions
**If you are encountering issues with AdAway blocking ads, working with a specific app, being disabled, etc., then please _READ_ this in its entirety BEFORE creating an issue!**

## How to Log DNS Requests

1. Start AdAway and go to the Menu.
2. Select "Log DNS Requests"
3. Click 'TCPDUMP IS NOT RUNNING!'
4. Wait until it shows 'TCPDUMP IS RUNNING!'
5. Open the App you wish to monitor for a while.  Click around on things and use the application as you normally would.
6. Go back to AdAway / Menu / Log DNS Requests and select 'OPEN LOG FILE'.
7. There you look for suspicious hostnames.
  1. REMOVE ADS: Try to block some of them by adding them to your Blacklist from that screen (long press a hostname), reapply AdAway and restart your Android device.
  2. FIX APPS THAT AREN'T WORKING: Look for some of the hosts the app will try to connect to and add to your Whitelist to allow it. (Keep in mind this will allow ANY app to connect to that URL to pull ads.)
8. If it helped and you are totally sure, which hostname served the ads, please report the hostname(s) in the Forum [Hosts Inbox](http://forum.hosts-file.net/viewforum.php?f=9) of [http://hosts-file.net](http://hosts-file.net) or in our [Issue tracker](https://github.com/dschuermann/ad-away/issues).

:: If you are not getting any logs showing up then the TCPDump process could be getting killed by SELinux enforcing policy.  You can go to the forums here, http://forum.xda-developers.com/ find your device thread and see if there is a way to get your device into SELinux Permissive state.  Then you can try the above again.

## Other things to do?
  * If you didn't succeed following the guide, you can also try to add a new issue and hope that somebody will help you: [Add issue](https://github.com/dschuermann/ad-away/issues)
  * Some apps have bundled the advertisements, use direct IP, or go through their own proxy. Thus you will never get rid of these ads by using AdAway.