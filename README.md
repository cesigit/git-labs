# git-labs
Several git labs for training purpose



Note: 
How to keep your ssh connection alive
```shell script
  sudo vi /etc/ssh/sshd_config
```
 uncomment these lines and change the values
```
ClientAliveInterval 120
ClientAliveCountMax 720
```
And restart the sshd daemon
```shell script
   sudo systemctl restart sshd
``` 

