# desafio-aws-cloudformation-dio
O projeto "desafio-aws-cloudformation-dio" propõe a implementação de uma pilha AWS utilizando CloudFormation como parte de um desafio prático. O objetivo é servir de apoio para estudos e futuras implementações em AWS, com notas e insights adquiridos durante a prática.

O arquivo principal do projeto é um template YAML do AWS CloudFormation que automatiza a criação dos seguintes recursos:

 * Security Group : Controle o acesso à instância EC2, permitindo conexões SSH (porta 22) apenas de um bloco IP específico e acesso HTTP (porta 80) globalmente.
 * Cluster ECS : Crie um cluster ECS chamado "MeuClusterECS".
 * Instância EC2 : Fornece uma instância EC2 do tipo t3.micro, definida para integrar-se ao ECS Cluster, utilizando uma AMI específica, associada ao Security Group e uma sub-rede definida.
 * IAM Role e Instance Profile : Configure uma role para permitir que uma instância EC2 interaja com o ECS, vinculando-a através de um Instance Profile.
 * Outputs : Ao final da execução, o template disponibiliza o nome do cluster ECS e o IP público da instância criada.

 * Resumo
   
    Este projeto demonstra uma solução simples e funcional para provisionar os recursos mínimos necessários para iniciar cargas de trabalho em ECS utilizando EC2, com boas práticas de segurança e automação via IaC (Infraestrutura como Código).
