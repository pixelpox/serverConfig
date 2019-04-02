# Backup and pull config for pihole

## Backup (push setting)

```bash
#following files are 544 root:root
scp /etc/dnsmasq.d/04-pihole-static-dhcp.conf simon@disco:/volume1/config/server/pihole/
scp /etc/hosts simon@disco:/volume1/config/server/pihole/
scp ~/pushPullConfig.md simon@disco:/volume1/config/server/pihole/
```

## Update (pull settings)

```bash
scp simon@disco:/volume1/config/server/pihole/04-pihole-static-dhcp.conf /etc/dnsmasq.d/04-pihole-static-dhcp.conf
scp simon@disco:/volume1/config/server/pihole/hosts /etc/hosts
scp simon@disco:/volume1/config/server/pihole/pushPullConfig.md ~/pushPullConfig.md
```