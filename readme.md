***
1. ssh -i ~/.ssh/appuser -J appuser@84.201.132.115  appuser@10.128.0.23
user | hostname | IP
appuser | bastion | 84.252.131.208
appuser | someinternalhost | 10.128.0.23
***
2. Необходимо создать файд ~/.ssh/config
Пример заполнения
host bastion
        hostname 84.201.132.115
        user appuser

host someinternalhost
        hostname 10.128.0.23
        user appuser
***

bastion_IP = 84.252.131.208  
someinternalhost_IP = 10.128.0.23  
