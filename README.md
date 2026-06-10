# Explorando Workflows Automatizados com AWS Step Functions

## Objetivo do Projeto

Este repositório foi criado como parte do desafio da DIO no bootcamp GFT - Fundamentos de Cloud com AWS.

O objetivo foi praticar a criação de workflows automatizados utilizando o AWS Step Functions integrado com funções AWS Lambda.

## Serviços Utilizados

- AWS Step Functions
- AWS Lambda
- IAM
- AWS Management Console

## O que é AWS Step Functions?

O AWS Step Functions é um serviço da AWS utilizado para criar fluxos de trabalho automatizados.

Ele permite organizar várias etapas de um processo, conectando diferentes serviços da AWS, como funções Lambda.

## O que é AWS Lambda?

O AWS Lambda é um serviço serverless que permite executar código sem precisar gerenciar servidores.

Neste projeto, as funções Lambda representam etapas de um fluxo de pedido.

## Fluxo Criado

O fluxo simula o processamento de um pedido.

Etapas:

1. ValidarPedido
2. VerificarEstoque
3. EnviarConfirmação

## Arquitetura do Workflow

Usuário inicia execução

↓

AWS Step Functions

↓

Lambda ValidarPedido

↓

Lambda VerificarEstoque

↓

Lambda EnviarConfirmação

↓

Fim da execução

## Prints do Projeto

### Funções Lambda Criadas

![Funções Lambda Criadas](images/lambda-functions.png)

### Máquina de Estado Criada

![Máquina de Estado Criada](images/state-machine-created.png)

### Workflow no Step Functions

![Workflow no Step Functions](images/workflow-step-functions.png)

### Execução com Sucesso

![Execução com Sucesso](images/execution-succeeded.png)

## Aprendizados

Durante este laboratório, aprendi que o AWS Step Functions permite orquestrar múltiplas funções Lambda em um fluxo visual e organizado.

Também entendi que cada etapa do workflow pode representar uma ação específica dentro de um processo maior, como validação de pedido, verificação de estoque e envio de confirmação.

## Conclusão

O AWS Step Functions é uma ferramenta importante para automação de processos na AWS, principalmente quando precisamos coordenar várias etapas ou serviços de forma organizada, escalável e visual.
