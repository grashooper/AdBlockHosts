# Common Problems with Solutions
**If you are encountering issues with AdAway blocking ads, working with a specific app, being disabled, etc., then please _READ_ this in its entirety BEFORE creating an issue!**

## Common Problems

## **AdAway has made my device/app crash**
  
For the record, AdAway doesn't cause any app to crash, nor does it prevent any ad from being displayed. It merely provides a mechanism to simplify the tedious process of editing the hosts file manually. What really matters is which URLs are redirected via that hosts file. Those URLs come from either the hosts sources that you ask AdAway to download and apply, or from any whitelist or blacklist you may have created. Don't blame or credit AdAway for your selection of URLs, it merely does what you ask it (unknowingly?) to do... 

For example, if you have an app that crashes when AdAway is enabled but runs fine without it, enable the convenient [[DNS Requests Log|LogDNS]] and find out which URLs that particular app needs to access. The default lists are useful starting points but they may be overly aggressive or let too many ads through. Loading more lists is not necessarily a wise option. There may be no universal answers even when referring to a specific app since it often depends on your ISP, location, settings, etc. In other words, simply asking here what to do to allow "MyRandomApp" to run can only bring you guesses from others and if they don't work in your case, look at your own DNS log, on your own device, while running your own copy of "MyRandomApp". Spend a few minutes understanding the basic wildcard mechanism (not specific to AdAway) and you'll be able to quickly enable or disable any URL you desire.

Note that none of that matters if an app bypasses the hosts mechanism and calls a numeric IP directly, builds in their own ads or leverages a proxy. Those direct calls, common in some games, don't go through DNS at all and therefore can't be altered by AdAway or the hosts file. The same applies to processes that use an external DNS resolution scheme, such as the Chrome proxy ("reduce bandwidth usage") or the DNS bypass used by some ISPs (Satellite providers, for example). 

## AdAway makes my device sluggish
  AdAway actually never 'runs' and takes virtually no resources.  Chances are your device may only be sluggish if you've loaded an extremely large hosts file.  You could completely delete AdAway but as long as you keep the same huge hosts file, chances are you'll notice some sluggishness especially on slower or resource-bound devices. Keep in mind that AdAway does very little except while it's actively downloading/merging fresh copies of the ads list. Unless it's awakened by the (optional) daily update alarm, it simply (optionally) redirects some requests to its localhost web server which has almost no impact on performance besides speeding up web page load time. It's almost impossible for AdAway itself to make your device sluggish.

I know some people are constantly trying to create ever expanding ads lists but such endeavors are often counterproductive. You can probably achieve the same results with some basic lists targeting the most common ad sites (the default lists suggested by AdAway, for example) and only adding a handful of wildcards to take care of your specific needs. There is absolutely no need to bog down your DNS requests by "blocking" sites you'll never visit or sites that disappeared a long time ago. One of my many pet peeves with those huge lists is that they typically add entries constantly but very seldom purge obsolete data. There is no point in having thousands of entries and only a few hundred (at most) that are actually likely to try to serve you an ad.

Yes, LESS is MORE!

## AdAway is enabled but all Ads are getting through!
  *Things to check:*
1. If you enabled Chrome's "Data Saver" option all requests in chrome will be going through a special proxy, making it impossible for AdAway to redirect anything. Set any data saver options in Chrome or ANY other browser to off or disabled.
2. Check your mobile network APN settings for any proxy, the proxy itself could be allowing ads. Disable the proxy.
3. If you are running on a custom ROM, check for Privacy Guard or any other built in Ad blockers. Remove them in the ROM settings and check /system/etc/ for any other hosts files.  Delete them and re-apply AdAway.
4. If you are on a corporate Wifi network or hotspot, it may be using its own proxy.  Turn off wifi to use your cellular at these locations if you need/want ads blocked.

## Every time I open AdAway it is disabled
  This will typically be incorrect root access or no write access to system.  Ad blocking is not accomplished by AdAway itself. It's done when an application queries your /system/etc/hosts file looking for the address of a host. That file may or may not have been built by AdAway. If all your ads are reappearing, either your hosts file has reverted to default (basically blocks nothing), or you are going through a proxy that ignores the hosts file. 

Verify that your hosts file contains more than the few default entries. If it doesn't, have AdAway try to edit it again, reboot and check again. If it still fails then you are unable to write to the system partiition and you need to check that you have full root and that system changes survive a reboot (S-OFF if you have an HTC device).
If the hosts file looks correct, delete any proxy from your APN and make sure your browser (Chrome?) doesn't have a proxy of its own.
Remember that after making any change to the hosts file or the proxy settings, you must reboot for the changes to take effect.

## Other things to do?
  * If you didn't succeed following the guide, you can also try to add a new issue and hope that somebody will help you: [Add issue](https://github.com/dschuermann/ad-away/issues)
  * Some apps have bundled the advertisements, use direct IP, or go through their own proxy. Thus you will never get rid of these ads by using AdAway.