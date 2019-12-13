# How to set up ansible for wordpress

## Requirement
### `labx.example.com & serverx.example.com install ansible git`

## Login by `user centos` at labx.example.com

#### - Run playbook setup-environment-labx.yml
``` bash
$ ansible-playbook -k --ask-become-pass setup-environment-labx.yml
```
#### - Run playbook setup-environment-server.yml
``` bash
$ ansible-playbook -k --ask-become-pass setup-environment-server.yml
```
> Note: Enter password `centos` 2 times

## Use playbook 
``` bash
$ ansible-playbook --ask-become-pass wordpress.yml
```

### Use playbook by roles
```bash
$ ansible-playbook roles_install_WP.yml --ask-become-pass -k
```
Run ซ้ำได้จ้าา
