# Xiaomi
Block xiaomi tracking you

> Assuimg you are root user oe executing via sudo

```
apt-get update
apt-get install squid3
cd /etc/squid
wget https://raw.githubusercontent.com/harikt/xiaomi/master/blacklist.acl
wget https://raw.githubusercontent.com/harikt/xiaomi/master/squid.conf
```

Start / Restart when ever you made any changes.

```
systemctl start squid
systemctl restart squid
```

## References 

1. https://github.com/hidden-refuge/spi
2. https://www.configserverfirewall.com/ubuntu-linux/install-squid-ubuntu-server/
