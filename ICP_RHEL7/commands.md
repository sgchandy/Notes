
###### Remove existing docker images #######

```bash
docker rm $(docker ps -a -q)
docker rmi $(docker images -q)
```


###### Remove existing docker images #######

```bash
mkdir /opt/icp
cd /opt/icp
docker run -v $(pwd):/data -e LICENSE=accept ibmcom/icp-inception:3.1.0 cp -r cluster /data
```


###### Generate SSH Keys #######

```bash
ssh-keygen -b 4096 -f ~/.ssh/id_rsa -N ""
cat ~/.ssh/id_rsa.pub | sudo tee -a ~/.ssh/authorized_keys
cp ~/.ssh/id_rsa ssh_key
```


###### Make changes to the config.yaml and hosts file (set IP Address) #######

```bash
vi config.yaml
vi hosts
```

###### Install Ansible ######
```bash
yum install ansible
cd /etc/ansible/
vi hosts

# ip_address ansible_user=root
# hostname ansible_user=root
```

###### Install ICP 3.1.0 ######
```bash
cd /opt/icp
docker run -e LICENSE=accept --net=host --rm -t -v $(pwd):/installer/cluster ibmcom/icp-inception:3.1.0 install -vvv
```
