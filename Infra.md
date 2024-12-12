## isv infra

--- switch
--- s3
--- s2
--- s1

--- belly
--- ups

### core services
1. [Proxmox](https://86.123.115.197:8006/) - hypervisor - root@86.123.115.197 / passwd
2. [cPanel](https://ns1.iservit.ro:2087/) - WHM / ~50 conturi cu mails, site uri de prezentare, tot felu
3. [snak](86.123.115.197:1194) - vpn service
4. [ted](86.123.115.199) - nginx server in front of pow / sls / copacei.ro / brilliantmeses.ro / hotelbrilliantplaza.ro
5. [web1](10.10.1.30) - copacei.ro / brilliantmeses.ro / hotelbrilliantplaza.ro

### psql db's
1. [db.pow](10.10.1.216)
2. [db.sls](10.10.1.133)

### k8s
- all pow/sls microservices are here
