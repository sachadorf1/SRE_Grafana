# SRE_Grafana
# Grafana
- Create an instance with port 3000 access and ssh from your ip
- ssh into instance
```
sudo apt-get install -y adduser libfontconfig1
wget https://dl.grafana.com/enterprise/release/grafana-enterprise_8.1.5_amd64.deb
sudo dpkg -i grafana-enterprise_8.1.5_amd64.deb
```
- Go into sources.list file:
`sudo nano /etc/apt/sources.list`
- Add `deb https://packagecloud.io/grafana/stable/debian/ stretch main` to the end of the file (last line)
- Save and close
```
curl https://packagecloud.io/gpg.key | sudo apt-key add -
sudo wget https://s3-us-west-2.amazonaws.com/grafana-releases/release/grafana_5.2.4_amd64.deb
sudo apt-get install grafanasudo systemctl daemon-reload
sudo systemctl start grafana-server
sudo systemctl status grafana-server
sudo systemctl enable grafana-server.service
sudo service grafana-server start
systemctl status grafana-server.service
```