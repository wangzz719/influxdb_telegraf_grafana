# Telegraf
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
