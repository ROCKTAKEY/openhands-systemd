# OpenHands on systemd
## Install
```shell
git clone https://github.com/ROCKTAKEY/openhands-systemd /root/openhands-systemd
cd /root/openhands-systemd
ln -s /root/openhands-systemd/systemd/openhands.service /etc/systemd/system/openhands.service
systemctl enable openhands.service
systemctl start openhands.service
```
## Update
```shell
cd /root/openhands
git pull origin main
systemctl daemon-reload
systemctl restart openhands.service
```
