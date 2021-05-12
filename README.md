

# Docker Compose Php MySQL
## _Infrastructure and Cloud Computing - MBA ES21_

## Desafio

> Subir dois pods, nginx e mysql, mapeando a porta 80 do nginx para acesso externo ao cluster e permitir que o contêiner do nginx tenha comunicação de rede no contêiner mysql pela porta 3306. 
A atividade pode ser feita localmente (minikube), AKS (Azure), EKS (AWS) ou no GKE (GCP). 
Se quiser criar o cluster nuvem Kubernetes com Terraform é opcional. 

## Tech

Tecnologias utilizadas

- [MySQL](https://www.mysql.com/) - O MySQL é um sistema de gerenciamento de banco de dados, que utiliza a linguagem SQL como interface
- [Kubernetes](https://www.docker.com/) - Kubernetes é um sistema de orquestração de contêineres open-source que automatiza a implantação, o dimensionamento e a gestão de aplicações em contêineres
- [PHP](https://www.php.net/) - PHP é uma linguagem interpretada livre, usada originalmente apenas para o desenvolvimento de aplicações presentes e atuantes no lado do servidor, capazes de gerar conteúdo dinâmico na World Wide Web
- [nginx](https://www.nginx.com/) - Nginx é um servidor leve de HTTP

## Instalação
#### 1- Passo

```sh
mkdir kuber && cd kuber
git clone https://github.com/jeffersonclark1/Kubernetes.git
```
#### 2- Passo
```sh
az login -u <email> -p <senha>
az aks get-credentials --resource-group <ResourceGroup> --name <ClusterName>
```

#### 3- Passo
```sh
kubectl apply -f ./
```

> IP Externo no Cluster
#### 4- Passo
```sh
kubectl get all 
```

## License

MIT

**Let's GO**