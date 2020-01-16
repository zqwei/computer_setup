## Sync files

rsync --remove-source-files -azvP /source/files /dest/files


## Set remote desktop

```bash
sudo vim /etc/services
# add -- xvncserver      5950/tcp                # VNC xinetd GDM base
sudo systemctl enable vncserver@1.service
sudo systemctl daemon-reload
sudo systemctl start vncserver@1.service
```
