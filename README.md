# Kibana4_init

This script runs as the kibana user.

Here are the commands that I'm using to setup this up.
```
umask 022
useradd -c "Kibana4 service user" -d /opt/kibana --system -s /sbin/nologin -U kibana
mkdir /var/run/kibana
mkdir /var/log/kibana
chown kibana.kibana /var/run/kibana /var/log/kibana
```
