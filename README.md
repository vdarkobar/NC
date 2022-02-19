<p align="left">
  <a href="https://github.com/vdarkobar/npm">Home</a>
  <br><br>
</p> 
  
# NextCloud 
  
Login to <a href="https://dash.cloudflare.com/">CloudFlare</a> and set *Domain name*, or *Domain name* and *Subdomain* for your *NextCloud*.
```
    A | example.com | YOUR WAN IP
```
or:
```
    A | example.com | YOUR WAN IP
```
```
    CNAME | subdomain | @ (or example.com)
```
Add subdomain *code* for Collabora Office:
```
    CNAME | code | @ (or example.com)
```
---
  
#### *Decide what you will use for*:
```
Time Zone, Domain name, Subdomain (if planned),
Local IP Address, NextCloud Admin username,
Collabora username, NextCloud Port Number.
```
  
### *Run this command*:
```
RED='\033[0;31m'; echo -ne "${RED}Enter directory name: "; read NAME; mkdir -p "$NAME"; \
cd "$NAME" && git clone https://github.com/vdarkobar/NC.git . && \
chmod +x setup.sh && \
./setup.sh
```
  
*Change Container names/Port numbers, if multiple instances are planed.*
  
### Log:
```
sudo docker-compose logs nextcloud-db
sudo docker-compose logs nextcloud
sudo docker-compose logs code
sudo docker logs -tf --tail="50" nextcloud-db
sudo docker logs -tf --tail="50" nextcloud
sudo docker logs -tf --tail="50" code
``` 
  
### Follow <i><a href="https://github.com/vdarkobar/NPM/blob/main/shared/NC%20Additional%20Settings.md">this link</a></i> for important NextCloud settings.  
  
