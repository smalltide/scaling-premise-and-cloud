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

Vagrant-Cassandra-DigitalOcean (On-Premise)  
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