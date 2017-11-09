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

# Manage Git 
'''
>First 
>  704  git init
>  705  git add .
>  706  git commit -m "First commit"
>  707  git remote add origin https://github.com/jcsou/ansible-infra.git
>  708  git remote -v
>  709  git push origin master
  
>Changement : 
>  713  git add .
>  714  git commit -m "First commit"
>  715  git push origin master
'''
