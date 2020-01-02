# GeoLite2 Database Mirror

GeoLite2 Database (GeoIP 2 Lite) mirror of last December 24th, 2019 updated version.

* GeoLite2-ASN.tar.gz
* GeoLite2-City.tar.gz
* GeoLite2-Country.tar.gz

CSF Firewall GeoLite2 Database files as at December 23rd, 2019 which are saved at `/var/lib/csf/Geo/`. You'd need to adjust `CC_INTERVAL = "14"` interval in `/etc/csf/csf.conf`

```
ls -lAh /var/lib/csf/Geo/   
total 16M
-rw------- 1 root root   55 Dec 23 19:00 COPYRIGHT.txt
-rw------- 1 root root  13M Dec 23 19:00 GeoLite2-Country-Blocks-IPv4.csv
-rw------- 1 root root 3.8M Dec 23 19:00 GeoLite2-Country-Blocks-IPv6.csv
-rw------- 1 root root 9.7K Dec 23 19:00 GeoLite2-Country-Locations-en.csv
-rw------- 1 root root  433 Dec 23 19:00 LICENSE.txt
-rw------- 1 root root  116 Dec 23 19:00 README.txt
```
```
# This option tells lfd how often to retrieve the MaxMind GeoLite2 Country
# database for CC_ALLOW, CC_ALLOW_FILTER, CC_DENY, CC_IGNORE and CC_LOOKUPS (in
# days)
CC_INTERVAL = "14"
```
