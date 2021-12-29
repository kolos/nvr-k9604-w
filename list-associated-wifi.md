Lists associated wifi clients info

```bash
# cat /proc/net/rtl8188eu/wlan0/all_sta_info
sta_dz_bitmap=0x0, tim_bitmap=0x0
==============================
sta's macaddr:de:ad:be:ef:00:01
rtsen=0, cts2slef=0
state=0x10, aid=0, macid=32, raid=0
qos_en=1, ht_en=1, init_rate=0
bwmode=0, ch_offset=0, sgi_20m=1,sgi_40m=1
ampdu_enable = 1
agg_enable_bitmap=0, candidate_tid_bitmap=0
sleepq_len=0
sta_xmitpriv.vo_q_qcnt=0
sta_xmitpriv.vi_q_qcnt=0
sta_xmitpriv.be_q_qcnt=0
sta_xmitpriv.bk_q_qcnt=0
capability=0x0
flags=0x0
wpa_psk=0x0
wpa2_group_cipher=0x0
wpa2_pairwise_cipher=0x0
qos_info=0x0
dot118021XPrivacy=0x0
==============================
==============================
sta's macaddr:ff:ff:ff:ff:ff:ff
rtsen=0, cts2slef=0
state=0x1, aid=0, macid=1, raid=6
qos_en=0, ht_en=0, init_rate=3
bwmode=0, ch_offset=0, sgi_20m=0,sgi_40m=0
ampdu_enable = 0
agg_enable_bitmap=0, candidate_tid_bitmap=0
sleepq_len=0
sta_xmitpriv.vo_q_qcnt=0
sta_xmitpriv.vi_q_qcnt=0
sta_xmitpriv.be_q_qcnt=0
sta_xmitpriv.bk_q_qcnt=0
capability=0x0
flags=0x0
wpa_psk=0x0
wpa2_group_cipher=0x0
wpa2_pairwise_cipher=0x0
qos_info=0x0
dot118021XPrivacy=0x4
==============================
```
