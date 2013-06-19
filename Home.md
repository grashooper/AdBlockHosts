# AdAway

## User information
[[Other Hosts Sources|HostsSources]]
[[How to block new ads|BlockNewAds]]
[[List of problematic applications|ProblematicApps]]

## Advanced Information
[[Hosts file Syntax|HostsSyntax]]


## Facts

Some facts I found out about Androids hosts file, thought they might be interesting...

  * Hosts file gets recognized immediately by the operating system, but Java has its own DNS cache: http://stackoverflow.com/questions/4175066/android-hosts-file-usage , so we need to restart Android

  * "When I use jager rom I have to use /data/hosts instead of /data/data/hosts. Something happens to /data/data after the phone reboots making /data/data/hosts inaccessible. Make sure you symlink the new location with "ln -s /data/hosts /system/etc/hosts" and leave the check box unchecked when running adfree. " ( http://androidforums.com/application-development/240927-android-emulator-edit-hosts-file-doesnt-resolve-custom-domain-name.html )

  * HTC phones have S-ON, see http://www.addictivetips.com/mobile/what-is-s-off-how-to-gain-it-on-htc-android-phones-with-unrevoked-forever/ . Then system-Partition can not be written