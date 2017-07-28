# Grafana Installation
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