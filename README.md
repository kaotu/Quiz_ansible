# How to set up ansible for wordpress

## Login by `user centos` at labx.example.com
#### 1. Create ssh key and copy pub key to server
``` bash
ssh-keygen
ssh-copy-id centos@serverx.example.com
```
#### 2. Update hosts at /etc/hosts
``` bash
sudo vim /etc/hosts
   192.168.52.140 labx labx.example.com
   192.168.52.141 serverx serverx.example.com
```

## Login by `user root` at serverx.example.com
#### 1. Add group wheel for user centos
``` bash
usermod -aG wheel centos
```
#### 2. Update hosts at /etc/hosts
``` bash
sudo vim /etc/hosts
   192.168.52.140 labx labx.example.com
   192.168.52.141 serverx serverx.example.com
```
