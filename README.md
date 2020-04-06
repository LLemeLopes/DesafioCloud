# Desafio Cloud
**Scripts de automação utilizados**

Para Deploy do ambiente seguir a seguinte ordem de execução:
> 1. cf-NetworkStack.yaml (Deploy de todas as peças de rede)
> 1. cf-ClusterStack.yaml (Deploy do Cluster Fargate e Load Balancer)
> 1. cf-ServiceStack.yaml (Deploy da Task Definition e Serviço - Camada Aplicacao )
> 1. cf-SNSStack.yaml (Deploy do topico SNS para Scheduler)
> 1. cf-RepositoryStack.yaml (Deploy da camada de Banco de Dados)
> 1. cf-EC2Bastion.yaml (Deploy EC2 Bastion Host)

Para validar a camada de aplicação (Container Fargate), conectar no Bastion Host e executar o comando:

`curl http://EnderecoDNSdoBalancer:PortaListener`.

O Resultado deverá ser o seguinte: **It works!**
