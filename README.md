# SSHCPanelGithub

## This repo contains the command for creating SSH file and allow permission use for Github and this help to connect private Git repo with CPanel.

### ssh-keygen -t rsa -b 4096 -C "techrev2@techrevivals.net"
### touch ~/.ssh/config
### chmod 0600 ~/.ssh/config
### chown techrev2:techrev2 ~/.ssh/config
### ssh -T git@github.com

### .cpanel.yml
```yml
deployment:
    task:
    - export DEPLOYPATH=/home2/techrev2/coded.money.techrevivals.net
    - /bin/cp * $DEPLOYPATH
```
