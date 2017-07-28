# Welcome To The Server Monitor Using: Influxdb + Telegraf + Grafana Wiki
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
wget https://dl.influxdata.com/influxdb/releases/influxdb-1.3.1.x86_64.rpm
sudo yum localinstall influxdb-1.3.1.x86_64.rpm
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

#Telegraf
## Install Telegraf V1.3.5
### OS X (via Homebrew)
```
brew update
brew install telegraf
```
### Docker Image
```
docker pull telegraf
```
### Ubuntu & Debian
```
wget https://dl.influxdata.com/telegraf/releases/telegraf_1.3.5-1_amd64.deb
sudo dpkg -i telegraf_1.3.5-1_amd64.deb
```
### ReadHat & CentOS
```
wget https://dl.influxdata.com/telegraf/releases/telegraf-1.3.5-1.x86_64.rpm
sudo yum localinstall telegraf-1.3.5-1.x86_64.rpm
```
### Linux Binaries (64-bit)
```
wget https://dl.influxdata.com/telegraf/releases/telegraf-1.3.5_linux_amd64.tar.gz
tar xvfz telegraf-1.3.5_linux_amd64.tar.gz
```
### Reference
```
For more install instruction see: https://portal.influxdata.com/downloads
```
## Start Telegraf Service
```
systemctl start telegraf.service
```
You can edit `/etc/telegraf/telegraf.conf` to use coustom configuration.

# Grafana
## Install Grafana V4.4.1
### OS X (via Homebrew)
```
brew update
brew install grafana
```
### Docker Image
```
docker run -i -p 3000:3000 grafana/grafana
```
### Ubuntu & Debian
```
wget https://s3-us-west-2.amazonaws.com/grafana-releases/release/grafana_4.4.1_amd64.deb
sudo dpkg -i grafana_4.4.1_amd64.deb
```
### ReadHat & CentOS
```
wget https://s3-us-west-2.amazonaws.com/grafana-releases/release/grafana-4.4.1-1.x86_64.rpm
sudo yum localinstall grafana-4.4.1-1.x86_64.rpm
```
### Tips
#### urw-fonts required error
Install urw-fonts
```
wget ftp://rpmfind.net/linux/fedora-secondary/releases/26/Everything/s390x/os/Packages/u/urw-fonts-2.4-23.fc26.noarch.rpm
sudo yum localinstall urw-fonts-2.4-23.fc26.noarch.rpm
```

### Reference
```
For more install instruction see: http://docs.grafana.org/installation/
```
## Start Grafana
```
systemctl start grafana-server
```