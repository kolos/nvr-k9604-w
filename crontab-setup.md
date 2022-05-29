# Setup crontab for logging data
temperature sensor & connected wifi clients

```bash

killall crond
mkdir -p /tmp/cron

cat <<EOF >/tmp/log_temp
#!/bin/ash

now=\$(date)
id=1
target_ip="192.168.1.1"

temp_f=\$(devmem 0x20270110 32 0x60FA0000 ; devmem 0x20270114 8)
temp_c=\$(( ((\$temp_f*180)/256)-40 ))

wlan_macs=\$(cat /proc/net/rtl8188eu/wlan0/all_sta_info | grep -c macaddr)
wlan_connected=\$(( \$wlan_macs - 2 ))

wget "http://\$target_ip/log_camera?id=\$id&val=\$temp_c&macs=\$wlan_connected" -O /dev/null -T 1 > /dev/null 2>&1

echo "\$now \$id \$temp_c \$wlan_connected" > /dev/kmsg
EOF

chmod +x /tmp/log_temp
echo "*/5 * * * * /tmp/log_temp" > /tmp/cron/root
crond -c /tmp/cron

```

