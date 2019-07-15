## GCP & Godaddy Domain Link

+ GCP Compute Engine / VM instance / Create an instance 
     - f1-micro - Minimum (about $0.007 hourly, $5.22 monthly estimate)
     - Debian GNU/Linux 9 (stretch) - Basic one
     - Allow HTTP traffic
     - Allow HTTPs traffic
     
---

+ GCP Compute Engine / VM instance 
     - Connect SSH
     - sudo su (get admin auth)
     - apt-get update 
     - apt-get install apache2 (web server install)
     - /var/www/html/index.html file check
     - check with External IP by browser : External IP number only or http url (not https)
     
---

+ GCP Network services / Cloud DNS / Create a DNS zone
     - Zone type : public
     - Zone name : 'zone-name-example'
     - DNS name : 'www.xxxxxxxxx.com'   : put purchased domain name
     - DNSSEC : off (have no idea at the moment)
     - create
     
---

+ GCP Network services / Cloud DNS / Zone details (click the Zone name)
     - Add record set : 'DomainName.com' without www  & Pv4 address : 'External IP'
     - Add record set : 'WWW.DomainName.com' with www & Pv4 address : 'External IP'
     - copy 4 NS type data(*01)
     
---
+ Godaddy (if only there are purchased domain name)
     - [https://dcc.godaddy.com/domains/](https://dcc.godaddy.com/domains/)
     - DNS Manage
     - Name Server : Custom Type
     - Name Server : set GCP's 4 NS type data(*01) & make sure without '.' comma at the end of 4 NS type address)
     
     
---

+ Aftewards
     - waiting for 15minutes (officially 24 ~ 48 hours in case of Godaddy)
     - try Domain name with browser 
     - Cross finger !!
 
 