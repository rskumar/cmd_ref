## SSH
**List all SSH connections**
```
netstat -pant | grep 'ESTABLISHED.*sshd'
```
```
sudo netstat -atp | grep 'ESTABLISHED.*ssh' | awk '{print $5}'| sed 's/:ssh//'
```
