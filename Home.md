Welcome to the influxdb_telegraf_grafana wiki!
# Influxdb
## Install Influxdb V1.3.1
### OS X (via Homebrew)
```
brew update
brew install influxdb
```
### Docker Image
```
docker pull influxdb
```

### Ubuntu & Debian
```
wget https://dl.influxdata.com/influxdb/releases/influxdb_1.3.1_amd64.deb
sudo dpkg -i influxdb_1.3.1_amd64.deb
```
### ReadHat & CentOS
```
wget https://dl.influxdata.com/influxdb/releases/influxdb_1.3.1_amd64.deb
sudo dpkg -i influxdb_1.3.1_amd64.deb
```
### Linux Binaries (64-bit)
```
wget https://dl.influxdata.com/influxdb/releases/influxdb-1.3.1_linux_amd64.tar.gz
tar xvfz influxdb-1.3.1_linux_amd64.tar.gz
```
### Reference
```
For more install instruction see: https://portal.influxdata.com/downloads
```
## Start Influxdb Service
```
systemctl start influxdb.service
```
You can edit `/etc/influxdb/influxdb.conf` to use coustom configuration.

# telegraf

# grafana