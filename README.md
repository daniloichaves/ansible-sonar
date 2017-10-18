# sonar-backup

Inicializacao do ambiente

'''
docker run -it -p 2222:22 centos

docker run -it centos:centos6


docker run -d --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=sonar -e POSTGRES_DB=sonar -e POSTGRES_USER=sonar postgres:9.6.5

docker run -it -p 9000:9000 --link postgres:postgres centos:centos6



docker run -it -p 8080:8080  registry.access.redhat.com/rhel7/rhel


Adicionar o container id no aquivo sonar-playbook.yml

*shell* rodar o comando

Docker ambiente de desenvolvimento

'''
ansible-playbook -i "5e5e1c0b89c5," sonar-playbook.yml -vvv
'''


'''
deploy -c stack.yml postgres (or docker-compose -f stack.yml up), 
'''

Verificando conexão

ansible all -c ssh -i prod-host -m ping --user="x198754" --ask-pass


'''
sudo ansible-playbook -i prod-host --user="x198754" --ask-pass sonar-playbook.yml
'''


'''
sudo ansible-playbook -i prod-host --user="x198761" --ask-pass sonar-playbook.yml
'''



Confiuration path

*Backup*
```
/opt/sonar/backup
```



*Instalation*
'''
/var/lib/sonar
'''


Command Starting sonar inside container

'''
/etc/alternatives/java -Dcom.sun.akuma.Daemon=daemonized -Djava.awt.headless=true -Dsonar_HOME=/var/lib/sonar -jar /usr/lib/sonar/sonar.war --logfile=/var/log/sonar/sonar.log --webroot=/var/cache/sonar/war --httpPort=8080 --debug=5 --handlerCountMax=100 --handlerCountMaxIdle=20
'''
