# scaling-premise-and-cloud
Get experienced with Vagrant, DigitalOcean, Cassandra, AWS, Elastic Beanstalk, Terraform, Kubernetes, Deis, and Docker.

Learn DevOps: Scaling apps On-Premises and in the Cloud  
https://www.udemy.com/learn-devops-scaling-apps-on-premise-and-in-the-cloud
https://12factor.net/zh_cn/

Skills
1. Vagrant
2. DigitalOcean
3. Cassandra
4. AWS 
5. Elastic Beanstalk
6. Terraform
7. Kubernetes
8. Dokku
9. Deis
10. Docker

Git Repositories:
Cassandra: https://github.com/wardviaene/digitalocean-vagrant-cassandra-multi-node  
Devops Box: https://github.com/wardviaene/devops-box  
Terraform Demo: https://github.com/wardviaene/terraform-demo  
Docker PHP7: https://github.com/wardviaene/docker-php7  
Eb-php-example: https://github.com/wardviaene/eb-php-example  
Eb-php7-docker-example: https://github.com/wardviaene/eb-php7-docker-example  
Dokku demo: https://github.com/wardviaene/dokku-demo  
Deis demo: https://github.com/wardviaene/deis-demo  

![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/intro.png "intro")

Introduction and How to scale
```
  > https://12factor.net/zh_cn/
```
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/scalable1.png "scalable1")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/scalable2.png "scalable2")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/db1.png "db1")![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/db2.png "db2")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/IaaS-PaaS.png "IaaS-PaaS")

## Vagrant-Cassandra-DigitalOcean (On-Premise)  

Launching Cassandra with Vagrant on DigitalOcean
```
  > https://www.vagrantup.com/downloads.html
  > vagrant plugin install vagrant-digitalocean
  >
  > cd digitalocean-vagrant-cassandra-multi-node
  > ssh-keygen -f id_rsa
  > vagrant up
  > vagrant ssh node1
  > /opt/apache-cassandra-3.0.14/bin/nodetool status
  > tail -n100 /opt/apache-cassandra-3.0.14/logs/system.log
  > /opt/apache-cassandra-3.0.14/bin/cqlsh
  > /opt/apache-cassandra-3.0.14/bin/nodetool getendpoints test1 customers 1
  > /opt/apache-cassandra-3.0.14/bin/cqlsh
```
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/cqlsh.png "cqlsh")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/cqlsh2.png "cqlsh2")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/distribute-system.png "distribute-system")

## Amazon AWS with Elastic Beanstalk and Terraform  

Amazon AWS Virtual Private Networks (VPCs)
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/vpc1.png "vpc1")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/vpc2.png "vpc2")

Create AWS VPC with Terraform
```
  > https://aws.amazon.com/tw/free
  > create aws group and user on aws console
  > cd devops-box
  > vagrant up (build a vm install Terraform and Ansible and AWS CLI)
  > vagrant ssh devops-box
  > git clone https://github.com/wardviaene/terraform-demo (on devops-box vm)
  > git checkout vpc-demo
  > input AWS_ACCESS_KEY in terraform.tfvars
  > terraform plan
  > terraform apply (see creating vpc on aws)
```
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/tf5.png "tf5")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/tf1.png "tf1")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/tf2.png "tf2")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/tf3.png "tf3")
![alt text](https://github.com/smalltide/scaling-premise-and-cloud/blob/master/img/tf4.png "tf4")