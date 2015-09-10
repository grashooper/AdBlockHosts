# How to Log DNS Requests

1. Start AdAway and go to the Menu.
2. Select "Log DNS Requests"
3. Click 'TCPDUMP IS NOT RUNNING!'
4. Wait until it shows 'TCPDUMP IS RUNNING!'
5a. (Whitelist only): Go to the main screen and click the button to 'Disable Adaway'.  
5b. Open the App you wish to monitor for a while.  Click around on things and use the application as you normally would.
6. Go back to AdAway / Menu / Log DNS Requests and select 'OPEN LOG FILE'.
7. There you look for suspicious hostnames.
  1. REMOVE ADS (Blacklist): Try to block some of them by adding them to your Blacklist from that screen (long press a hostname), reapply AdAway and restart your Android device.
  2. FIX APPS THAT AREN'T WORKING (Whitelist): Look for some of the hosts the app will try to connect to and add to your Whitelist to allow it. (Keep in mind this will allow ANY app to connect to that URL to pull ads.)
8. (Whitelist only): Re-apply Adaway to see if your whitelist additions worked.  Remember if you see a bunch of similar host names like 'a.adserver.com', 'b.adserver.com', 'c.adserver.com'; you can just add one of them to your whitelist, long press on it to edit.  Then change to '*.adserver.com' to whitelist that whole domain.
9. If it helped and you are totally sure, which hostname served the ads, please report the hostname(s) in the Forum [Hosts Inbox](http://forum.hosts-file.net/viewforum.php?f=9) of [http://hosts-file.net](http://hosts-file.net) or in our [Issue tracker](https://github.com/dschuermann/ad-away/issues).

:: If you are not getting any logs showing up then the TCPDump process could be getting killed by SELinux enforcing policy.  You can go to the forums here, http://forum.xda-developers.com/ find your device thread and see if there is a way to get your device into SELinux Permissive state.  Then you can try the above again.