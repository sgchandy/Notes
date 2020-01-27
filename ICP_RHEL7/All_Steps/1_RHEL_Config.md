### Initial Configuration ###

##### Enable RHEL Subscriptions on machine (change enabled from 0 to 1)

```bash
# yum repolist all

# yum repolist

# vi /etc/yum.repos.d/redhat.repo
  

```

##### Identify IP Address (in this case the inet address of eth0
```bash
# ifconfig
```

###### Generate SSH Keys #######

```bash
ssh-keygen -b 4096 -f ~/.ssh/id_rsa -N ""
cat ~/.ssh/id_rsa.pub | sudo tee -a ~/.ssh/authorized_keys
cp ~/.ssh/id_rsa ssh_key
```
