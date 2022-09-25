# Visão geral

Imagem Docker e scripts auxiliadores para trabalhar com o AWS Command Line Interface [(AWS CLI)](https://aws.amazon.com/pt/cli/).

## Tecnologias

- [Docker](https://docs.docker.com/engine/reference/builder/) permite criar imagens automaticamente lendo as instruções de um arquivo Dockerfile. 

- [(AWS CLI)](https://aws.amazon.com/pt/cli/) é uma ferramenta unificada para o gerenciamento de seus produtos da AWS.

- [Shell script](https://pt.wikipedia.org/wiki/Shell_script), é o nome dado a um arquivo que será interpretado por algum programa tipo Shell.
 
# Setup da aplicação (local)

## Pré-requisito

Antes de rodar a aplicação é preciso garantir que as seguintes dependências estejam corretamente instaladas:
[Install Docker Engine](https://docs.docker.com/engine/install/)

## Construção e execução da imagem

Primeiramente, faça o build da imagem Docker:
```
docker build -f Dockerfile_awscli -t automacao-awscli .
```
Informe as credenciais de acesso ao usuário AWS IAM criado, no arquivo "credenciais_docker":
```
AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
```
Feito isso, rode o script sh:
```
sh run_docker.sh
```
Pronto. O container está disponível e configurado para utilização:
```
root@daccd300522d:/# 
```
