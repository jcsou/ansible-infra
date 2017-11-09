# install devops infra

## Command to install from empty centos
yum update
yum install libselinux-python
yum install epel-release
yum install ansible
==> 2.4 --->  yum localinstall ansible-2.4.0.0-1.el7.noarch.rpm

## use ansible to install 


## manage application 
service jenkins start | stop
service artifactory start | stop

## access aux apllicatifs
 jenkins
http://srv-devops:8088 

 artifact
http://srv-devops:8081


