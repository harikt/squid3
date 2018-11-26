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

## Configuration for Mobile Netwrorks

1. Settings
2. Sim cards and mobile networks
3. Provider
4. Access point names
6. Proxy => use your IP address
7. Port  => The one you have given to squid
8. Username => The one you created via `htpasswd -c /etc/squid3/passwd <username>`
9. Password => The password given for the above command

## Configuration for Wifi

1. Settings
2. Wifi
3. Proxy
4. Manual
5. Set IP address of the server
6. Port number

> If you are using browser it will prompt for username / password. Provide the one you have created via htpasswd command.

## References 

1. https://github.com/hidden-refuge/spi
2. https://www.configserverfirewall.com/ubuntu-linux/install-squid-ubuntu-server/
