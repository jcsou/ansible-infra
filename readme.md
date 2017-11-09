# install devops infra

## Command to install from empty centos
yum update
yum install libselinux-python
yum install epel-release
yum install ansible
==> 2.4 --->  yum localinstall ansible-2.4.0.0-1.el7.noarch.rpm

## use ansible to install 
ansible-playbook -i "localhost," -c local infradevops.yml

## manage application 
service jenkins start | stop

service artifactory start | stop

## firewall open on local vmware
sudo firewall-cmd --zone=public --add-port=8081/tcp --permanent

sudo firewall-cmd --zone=public --add-port=8088/tcp --permanent

sudo firewall-cmd --reload


## access aux apllicatifs
 jenkins

http://srv-devops:8088 

 artifact

http://srv-devops:8081

# Manage Git 
Quelques Commandes
```
First 
  git init
  git add .
  git commit -m "First commit"
  git remote add origin https://github.com/jcsou/ansible-infra.git
  git remote -v
  git push origin master
  
Changement : 
  git add .
  git commit -m "First commit"
  git push origin master
```
