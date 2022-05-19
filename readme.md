# GeoLite2 Database Mirror

GeoLite2 Database (GeoIP 2 Lite) mirror of May 17, 2022 updated version.

* GeoLite2-ASN.tar.gz
* GeoLite2-City.tar.gz
* GeoLite2-Country.tar.gz

CSF Firewall GeoLite2 Database files as at May 17, 2022 which are saved at `/var/lib/csf/Geo/`. You'd need to adjust `CC_INTERVAL = "14"` interval in `/etc/csf/csf.conf`

```
ls -lAh /var/lib/csf/Geo/
total 24M
-rw-rw-r-- 1 root root   55 May 16 08:00 COPYRIGHT.txt
-rw-rw-r-- 1 root root  14M May 16 08:00 GeoLite2-Country-Blocks-IPv4.csv
-rw-rw-r-- 1 root root  11M May 16 08:00 GeoLite2-Country-Blocks-IPv6.csv
-rw-rw-r-- 1 root root 9.7K May 16 08:00 GeoLite2-Country-Locations-en.csv
-rw-rw-r-- 1 root root  398 May 16 08:00 LICENSE.txt
-rw------- 1 root root  116 May 30  2021 README.txt
```
```
# This option tells lfd how often to retrieve the MaxMind GeoLite2 Country
# database for CC_ALLOW, CC_ALLOW_FILTER, CC_DENY, CC_IGNORE and CC_LOOKUPS (in
# days)
CC_INTERVAL = "14"
```
