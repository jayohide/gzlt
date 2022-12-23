组播地址
udpxy脚本
vim /etc/hotplug.d/iface/100-udpxy
#!/bin/sh

if [ "$INTERFACE" = "iptv" ] && [ "$ACTION" = "ifup" -o "$ACTION" == "ifupdate" ]
then
        /etc/init.d/udpxy restart
fi
