# Xiaomi
Block xiaomi tracking you

```
sudo apt-get update
sudo apt-get install squid3
cd /etc/squid
wget https://raw.githubusercontent.com/harikt/xiaomi/master/blacklist.acl
wget https://raw.githubusercontent.com/harikt/xiaomi/master/squid.conf
```

Start / Restart when ever you made any changes.

```
sudo systemctl start squid
sudo systemctl restart squid
```

## References 

1. https://github.com/hidden-refuge/spi
2. https://www.configserverfirewall.com/ubuntu-linux/install-squid-ubuntu-server/
