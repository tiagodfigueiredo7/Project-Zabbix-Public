# Projeto - Zabbix
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/tiagodfigueiredo7/awsterralt/blob/main/LICENCE) 

# Sobre o projeto

Nesse Projeto criamos toda infra AWS para ferramenta Zabbix, utilizando um Ec2.T2.Medium, um Rds-MariaDB - e DockerCompose para rodar containers,


##  Infra Cloud

- VPC
- SUBNET
- IAM
- E2 
- Docker 
- Compose 



#  Projeto 

![Web 1](https://github.com/tiagodfigueiredo7/assets/blob/main/WhatsApp%20Image%202022-06-28%20at%2009.00.20.jpeg)



## Tecnologias utilizadas

- Aws 
- Docker
- Compose
- GitHub
- Zabbix



## Pré-requisitos: 

Conta AWS



## Preparando a Infra

Instalações

- VPC 
- Internet Gataway
- Route-table
- Subnets


- us-east-1-A ( Virginia )
- us-esat-2-B ( Virginia )




## Criando EC2 e Rds 

- EC2 Amazon Linux
- RDS Free Tier


## Dentro do Servidor SSH

- MySql - MariaDB
Endpoint - RDS - Nome do EndpointRDS

```
yum install mysql
yum install nc
nc -zv prod-zabbix-db.(endpoint aws )3306

```
## Conectando no banco de Dados
Endpoint - RDS - Nome do EndpointRDS

```
mysql -u admin -h(endpoint Aws ) -p
password: xxxxxxxxxxxxx

```
## Criando usuario

```
CREATE USER 'zabbix'@'%' IDENTIFIED BY 'PASSWORD';

```



# Instalação  Docker ( Linux ) <img align="center" alt="Rafa-Python" height="70" width="80" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original-wordmark.svg">
https://docs.docker.com/desktop/linux/install/

```
yum update
yum install docker 
sudo usermod -aG docker $USER
systemctl status docker
systemctl start docker
yum install docker-compose 

```


## Criando pro Container Docker- Compose

- zabbix-server-mysql:
- zabbix-web-nginx-mysql:
- zabbix-java-gateway:
 
## Fotos do Projeto  


## Docker - Containers 

![Web 2](https://github.com/tiagodfigueiredo7/assets/blob/main/WhatsApp%20Image%202022-07-04%20at%2012.33.52.jpeg)


## Zabbix 


![Web 3](https://github.com/tiagodfigueiredo7/assets/blob/main/WhatsApp%20Image%202022-07-04%20at%2012.38.56.jpeg)





## Autor

Tiago Domingos Figueiredo 

https://www.linkedin.com/in/tiagodfigueiredo/


![Web 1](https://github.com/tiagodfigueiredo7/assets/blob/main/t.jpg)
