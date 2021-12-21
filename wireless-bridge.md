# Use camera's wifi as wireless bridge

- Plug power, network cables in

- Login to the device via telnet

- Create hostapd file

```bash
cat << EOF > /tmp/hostapd.conf
ctrl_interface=/tmp/hostapd
interface=wlan0
wmm_enabled=1
ht_capab=[SHORT-GI-20]
macaddr_acl=0
auth_algs=1
ignore_broadcast_ssid=0
wpa_pairwise=CCMP
rsn_pairwise=CCMP
driver=rtl871xdrv
beacon_int=100
max_num_sta=16
wpa_group_rekey=86400
eap_server=0
wps_state=0
uuid=12345678-9abc-def0-1234-56789abcdef0
device_name=RTL8188eu
manufacturer=Realtek
model_name=Wireless NVR
model_number=WLAN_EU
serial_number=12345
device_type=6-0050F204-1
os_version=01020300
config_methods=label display push_button keypad
ssid=your_ssid_here
wpa_passphrase=your_password_here
channel=13
hw_mode=g
ieee80211n=1
wpa=2
wpa_key_mgmt=WPA-PSK
EOF
```

- Configure network

```bash
kill `pidof hostapd`
/usr/share/ipcam/wifi_tools/hostapd -B /tmp/hostapd.conf

brctl addbr br0
ifconfig br0 192.168.0.2 netmask 255.255.255.0 up
brctl addif br0 wlan0
ifconfig wlan0 0.0.0.0
ifconfig eth0:1 down
ifconfig eth0:2 down

brctl addif br0 eth0
ifconfig eth0 0.0.0.0

# echo 1 > /proc/sys/net/ipv4/ip_forward
# ifconfig br0 192.168.0.3
# route add default gw 192.168.0.1
# echo "nameserver 192.168.0.1" > /etc/resolv.conf```
