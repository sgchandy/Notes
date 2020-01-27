


##### Primary documentation ##### 


https://github.com/ibm-cloud-architecture/refarch-privatecloud/blob/master/icp-on-rhel/README.md


https://developer.ibm.com/recipes/tutorials/ibm-cloud-private-on-rhel/

https://github.com/joshisa/icp-rhel-install


##### Disable firewall ##### 

https://linuxconfig.org/how-to-stop-start-and-disable-enable-firewall-on-redhat-7-linux-system


##### IBM Documentation #####

https://www.ibm.com/support/knowledgecenter/SSBS6K_2.1.0/installing/prep_cluster.html

https://www.ibm.com/support/knowledgecenter/en/SSBS6K_2.1.0.3/installing/install_containers.html

https://developer.ibm.com/recipes/tutorials/understanding-ibm-cloud-private-architecture-installation/


##### Opening Ports ##### 

https://linuxhint.com/open-port-80-centos7/

https://firewalld.org/documentation/howto/enable-and-disable-firewalld.html

https://www.sysadmit.com/2016/12/linux-deshabilitar-firewall-redhat-centos.html


##### IBM Cloud Private Containerized Me ##### 

https://containerized.me/introduction-to-ibm-cloud-private/


##### Commands #####


###### SSH Keys ######

```bash
ssh-keygen -b 4096 -f ~/.ssh/id_rsa -N ""

cat ~/.ssh/id_rsa.pub | sudo tee -a ~/.ssh/authorized_keys

cp ~/.ssh/id_rsa ssh_key
```

###### Installer ######
```bash
docker run -e LICENSE=accept --net=host --rm -t -v $(pwd):/installer/cluster ibmcom/icp-inception:3.1.0 install -vvv
```


###### Open Ports ######
```bash
sudo firewall-cmd --permanent --add-port=80/tcp

sudo firewall-cmd --permanent --add-port=179/tcp

sudo firewall-cmd --permanent --add-port=443/tcp

sudo firewall-cmd --permanent --add-port=2222/tcp

sudo firewall-cmd --permanent --add-port=2380/tcp

sudo firewall-cmd --permanent --add-port=3306/tcp

sudo firewall-cmd --permanent --add-port=4001/tcp

sudo firewall-cmd --permanent --add-port=4194/tcp

sudo firewall-cmd --permanent --add-port=4444/tcp

sudo firewall-cmd --permanent --add-port=4567/tcp

sudo firewall-cmd --permanent --add-port=4568/tcp

sudo firewall-cmd --permanent --add-port=5000/tcp

sudo firewall-cmd --permanent --add-port=5044/tcp

sudo firewall-cmd --permanent --add-port=5046/tcp

sudo firewall-cmd --permanent --add-port=8001/tcp

sudo firewall-cmd --permanent --add-port=8080/tcp

sudo firewall-cmd --permanent --add-port=8082/tcp

sudo firewall-cmd --permanent --add-port=8084/tcp

sudo firewall-cmd --permanent --add-port=8101/tcp

sudo firewall-cmd --permanent --add-port=8181/tcp

sudo firewall-cmd --permanent --add-port=8443/tcp

sudo firewall-cmd --permanent --add-port=8500/tcp

sudo firewall-cmd --permanent --add-port=8600/tcp

sudo firewall-cmd --permanent --add-port=8743/tcp

sudo firewall-cmd --permanent --add-port=8888/tcp

sudo firewall-cmd --permanent --add-port=9200/tcp

sudo firewall-cmd --permanent --add-port=9235/tcp

sudo firewall-cmd --permanent --add-port=9300/tcp

sudo firewall-cmd --permanent --add-port=9443/tcp

sudo firewall-cmd --permanent --add-port=18080/tcp

sudo firewall-cmd --permanent --add-port=24007/tcp

sudo firewall-cmd --permanent --add-port=24008/tcp

sudo firewall-cmd --permanent --add-port=35357/tcp

sudo firewall-cmd --permanent --add-port=500/tcp

sudo firewall-cmd --permanent --add-port=500/udp

sudo firewall-cmd --permanent --add-port=4500/udp

sudo firewall-cmd --permanent --add-port=10248-10252/tcp

sudo firewall-cmd --permanent --add-port=30000-32767/tcp

sudo firewall-cmd --permanent --add-port=49152-49251/tcp

```
