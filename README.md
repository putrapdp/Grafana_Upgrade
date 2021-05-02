# Grafana_Upgrade

stop manual all alerts

```
cd /var/lib/grafana
cp -rp grafana.db grafana.db.orig
systemctl status grafana-server.service
systemctl stop grafana-server.service

wget https://dl.grafana.com/oss/release/grafana-7.5.5-1.x86_64.rpm
sudo yum install grafana-7.5.5-1.x86_64.rpm

systemctl start grafana-server.service

```
